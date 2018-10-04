# facenet-tensorflow

python gen_eval_pickle.py
=> results.bin ,need to put in lfw.bin

python make_tfrecord.py --data_path ~/kevin/data_gen/train_dataset_small/ --img_size 112
=>~/kevin/data_gen/tfrecord/kevin.tfrecords ,need to put in train.tfrecords

python train_nets.py  --max_epoch=100 --train_batch_size=50  --model_type=1 --test_batch_size=50 --pretrained_model=/home/cnn/kevin/face_id/MobileFaceNet_Tensorflow/self_ckpt/ --ckpt_path=/home/cnn/kevin/
face_id/MobileFaceNet_Tensorflow/self_ckpt/
