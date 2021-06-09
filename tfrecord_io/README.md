
#### tfrecord/_io

this is an simple sample code to learn about tfrecord. It's a good start to learn about concepts, e.g. Example, Features, Dataset, serialize, deserialize.


the sample data is from cifar/_10. in the sample, I do:

* decode/deserialize Dataset to Examples

* encode/serialize Examples to Dataset

* decode cifar/_10.tfrecord to images

* encode images back to cifar/_10.tfrecord


`Dataset` and `Example` are abstract class, while `cifar/_10.tfrecord` and `raw images` are instances. 

an `Example` is a dict of `Feature`s, `image bytes` is one feature, `image label` is another feature in `cifar/_10.tfrecords`.

utils usually is about image bytes to numpy array e.t.c


#### ImageNet-tfrecord

this sample comes from public [build_imageNet_data.py](https://github.com/kmonachopoulos/ImageNet-to-TFrecord/blob/master/build_imagenet_data.py), but update to work with tf2, which encode 1030 frame of images into 1 tfrecord, with defined features(e.g. image/length, image/width, image/filename, image/encoded e.t.c.


also good to learn about processing data in batch, multi-threads e.g. Coordinator, QueueRunner



