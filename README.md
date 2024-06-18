# Munin plugin for elasticsearch

A useful Munin plugin for monitoring elasticsearch 1.x nodes in Perl.<br />
This original codes has out of maintenance, so I have started maintenance this plugin.

## Features

* Tested on Elasticsearch 7 will probably work on other versions
* Supports monitoring local and/or another hosts

## Plugins

* elasticsearch_cache - field and filter cache stats
* elasticsearch_cluster_shards - cluster shards stats
* elasticsearch_docs - document count
* elasticsearch_gc_time - garbage collection time stats
* elasticsearch_index_size - index size
* elasticsearch_index_total - index total count
* elasticsearch_jvm_memory - JVM heap/non-heap memory usage
* elasticsearch_jvm_pools_size - JVM pools size stats
* elasticsearch_jvm_threads - JVM thread stats
* elasticsearch_open_files - open files count

## Configuration

### Variables

* env.url - The url to the elasticsearch server defaults to http://localhost:9200

### Example Config

Before use, put these settings into munin configuration.

  * examples of munin config file 
    *  in the case of all plugin config into single file.<br />
      `/etc/munin/plugin-conf.d/munin-node`
    * in the case of creating file per plugins.<br />
      `/etc/munin/plugin-conf.d/elasticsearch`

##### example of custom host and port configuration

```
[elasticsearch_*]
env.url http://localhost:9200
```

## Author

* Original code by [@rafl](https://github.com/rafl) has imported from https://gist.github.com/2159398
* [Contributors to y-ken/munin-plugin-elasticsearch](https://github.com/y-ken/munin-plugin-elasticsearch/graphs/contributors)
* Updated by [@y-ken](https://github.com/y-ken)
* Updated by [@rwky](https://github.com/rwky)

## Licence

MIT License
