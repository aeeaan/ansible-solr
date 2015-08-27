correcthorse.solr
=========

An ansible role for installing solr 5.

Role Variables
--------------

| Variable		| Default							| Notes				|
| :---			| :---								| :---				|
| solr_version		| 5.3.0								|				|
| solr_mirror		| http://archive.apache.org/dist/lucene/solr			|				|
| solr_package_name	| "solr-{{ solr_version }}"					|				|
| solr_archive		| "{{ solr_package_name }}.tgz"					|				|
| solr_download_url	| "{{ solr_mirror }}/{{ solr_version }}/{{ solr_archive }}"	|				|
| solr_home		| /opt/solr	  		     	   			|				|
| solr_user		| solr								|				|
| solr_cloud		| false								| enable cloud mode		|
| solr_open_port	| false								| 	       			|
| solr_memory		| 512m								| java heap size		|

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.solr }

Dependencies
------------

- correcthorse.common

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)