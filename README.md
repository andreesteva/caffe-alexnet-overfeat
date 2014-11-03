caffe-alexnet-overfeat
======================

Generate random image buffers, instantiate hybrid alexnet-overfeat architecture, then begin training

do the following:
./main_random.sh solver_alexoverfeat.prototoxt

If the train, val, and random_train_leveldb, random_val_leveldb folders already exist, you can do:
./run_training.sh solver_alexoverfeat.prototxt

To change the input dimensions of the images:
Open GenerateImages.m and change the first two lines
note: if train, val, and random_train_leveldb, random_val_leveldb folders already exist, they will need to be deleted 
before main_random can be run again


Note: this is the same exact procedure for using the second version:
randomNewCaffe-LMDB/
This version works for the latest version of caffe (as of September 2014), and uses the LMDB file format of caffe as opposed to the leveldb version.
