
this is an simple sample code to learn about tfrecord. It's a good start to learn about concepts, e.g. Example, Features, Dataset, serialize, deserialize.


the sample data is from cifar/_10. in the sample, I do:

* decode/deserialize Dataset to Examples

* encode/serialize Examples to Dataset

* decode cifar/_10.tfrecord to images

* encode images back to cifar/_10.tfrecord


`Dataset` and `Example` are abstract class, while `cifar/_10.tfrecord` and `raw images` are instances. 

an `Example` is a dict of `Feature`s, `image bytes` is one feature, `image label` is another feature in `cifar/_10.tfrecords`.

utils usually is about image bytes to numpy array e.t.c


