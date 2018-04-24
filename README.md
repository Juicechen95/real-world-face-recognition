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


# GPU
 Facenet (Tensorflow)https://github.com/davidsandberg/facenet
 
 center face(resnet) https://github.com/ydwen/caffe-face
 
 normface https://github.com/happynear/NormFace
 
 open face (https://github.com/cmusatyalab/openface)
 
 
 
 # CPU
 
 seetaface (https://github.com/seetaface/SeetaFaceEngine)
 
 dlib (https://github.com/davisking/dlib-models)
 
 # Dataset
 
