correcthorse.solr
=========

An ansible role for installing solr 5.

Role Variables
--------------

| Variable		| Default							| Notes				|
| :---			| :---								| :---				|
| solr_version		| 5.1.0								|				|
| solr_mirror		| http://mirror.cogentco.com/pub/apache/lucene/solr		|				|
| solr_package_name	| "solr-{{ solr_version }}"					|				|
| solr_archive		| "{{ solr_package_name }}.tgz"					|				|
| solr_download_url	| "{{ solr_mirror }}/{{ solr_version }}/{{ solr_archive }}"	|				|
| solr_home		| /opt/solr	  		     	   			|				|
| solr_user		| solr								|				|

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