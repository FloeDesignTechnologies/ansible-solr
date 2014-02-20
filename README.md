Solr
====

A role to install Apache Solr.

Role Variables
--------------

The following variables can be used with the solr role:

* **solr_source**: URL where to retrieve Solr, defaults 'http://apache.openmirror.de/lucene/solr'.
* **solr_version**: Solr version to use, defaults to '4.6.1'.
* **solr_destination**: Where to install Solr, defaults to '/usr/local/src'
* **solr_home**: The path the Solr home directory, defaults to "{{solr_destination}}/solr/example".
* **solr_memory**: Maximum memory for the Solr process, defaults to '1024'.
* **solr_basename**: The basename of the retrieved Solr archive, defaults to "solr-{{solr_version}}".
* **solr_multicore_src**: (optional) The path to a Solr configuration dir used as replacement (through synlink) of the default `multicore` one.

Dependencies
------------

- The oracle7-java is used to install Java.

License
-------

BSD

Authors Information
-------------------

- Stephan Hochhaus <stephan@yauh.de> - [yauh.de](http://yauh.de)
- Pierre Buyle <buyle@pheromone.ca>