# real-world-face-recognition
some face recognition models based on GPU/CPU(intergrated with face detection and alignment)

# Comparison
| Baseline Model      | Accuracy(LFW) | GPU\CPU |Framework|Detection|alignment|
| ------------------- |:-----------------:|:-----------:|:-----------------:|:-----------------:|:-----------------:|
| [Facenet](https://github.com/davidsandberg/facenet)| 99.65%| GPU| Tensorflow|MTCNN|MTCNN
| [Openface](https://github.com/cmusatyalab/openface)   | 99.63%(in paper) 92.92%  |both  |dlib+opencv, C++|dlib|dlib|
| [Center Face(ResNet)](https://github.com/ydwen/caffe-face) | 99.03%            | gpu         |caffe|no|no|
|[normface](https://github.com/happynear/NormFace)|used for improving| gpu|caffe|MTCNN|MTCNN|
|[seetaface](https://github.com/seetaface/SeetaFaceEngine)|97.1%|cpu|no|yes|yes|
|[dlib](https://github.com/davisking/dlib-models)|99.38%|cpu|no|dlib|dlib|

Both Facenet and openface are the implementation of paper [facenet_2015](https://arxiv.org/pdf/1503.03832.pdf). In openface, the real accuracy is lower because of the bad detection of dlib.


# Recommandation

If you are under computation-limited environment(cpu only or embedded system), seetaface(v1 and v2) and dlib are prefered. Although they can not provide best accuracy, the running speed is fast enough.

If you have GPUs, the Facenet are recommanded. Beacause it is highly acdamical and technical supported.
 
 # train with Facenet
 [classifier training Inception-ResNet-v1](https://github.com/davidsandberg/facenet/wiki/Classifier-training-of-inception-resnet-v1) 
 
 # test with Facenet
 [validate on LFW](https://github.com/davidsandberg/facenet/wiki/Validate-on-LFW)

 
 # Dataset
 
https://github.intel.com/syao/multi-task-learning.git
