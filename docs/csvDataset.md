## Differences between make_csv_dataset and CsvDataset in Tensorflow

The most convenient way to handle Timeseries data is in the CSV-format. When using TFDatasets, there are two major options to create Datasets from CsvFiles. When I was looking for the differences between these functions, I could not find any concrete information on them. So I decided to write my first blog on the major differences I found during my use.

> #### NOTE: Tested on Tensorflow 2.0 Alpha
> The changes described below were tested on TF2.0 Alpha. [This article](https://www.tensorflow.org/alpha/guide/effective_tf2#api_cleanup) describes the major changes in TF2.0. The Dataset classes were moved from tf.contrib to tf.data (below are the links to their original pages).

> In TF2.0, the classes are under :
> - [tf.data.experimental.make_csv_dataset](https://www.tensorflow.org/versions/r2.0/api_docs/python/tf/data/experimental/make_csv_dataset#aliases)
> - [tf.data.experimental.CsvDataset](https://www.tensorflow.org/versions/r2.0/api_docs/python/tf/data/experimental/CsvDataset#class_csvdataset)


> Older Deprecated Functions :
> - [tf.contrib.data.make_csv_dataset](https://www.tensorflow.org/api_docs/python/tf/contrib/data/make_csv_dataset)
> - [tf.contrib.data.CsvDataset](https://www.tensorflow.org/api_docs/python/tf/contrib/data/CsvDataset)

So what really are the differences between them? I tried it out myself and below are the major findings.
