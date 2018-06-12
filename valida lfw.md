# align the LFW dataset
for N in {1..4}; do \
python src/align/align_dataset_mtcnn.py \
~/data/lfw/raw \
~/data/lfw/lfw_mtcnnpy_160 \
--image_size 160 \
--margin 32 \
--random_order \
--gpu_memory_fraction 0.25 \
& done


# run the test
python src/validate_on_lfw.py \
~/data/lfw/lfw_mtcnnpy_160 \
/home/lingzhitech/projects/jcz/facenet/pretrained_models/20180402-114759 \
--distance_metric 1 \
--use_flipped_images \
--subtract_mean \
--use_fixed_image_standardization
