# Diversity and Inclusion Metrics

This work was done during my summer Outreachy internship in Open Innovation Team, Mozilla with Emma Irwin as my Mentor.

## Contents
1. [Introduction](#introduction)
2. [Dependencies](#dependencies)
3. [Installation](#installation)
4. [Presentation](#presentation)
5. [Screenshots](#screenshots)

## Introduction
### Diversity and Inclusion

### Elasticsearch
Elasticsearch is a distributed RESTful search engine built for the cloud. Features include:

* Distributed and Highly Available Search Engine.
** Each index is fully sharded with a configurable number of shards.
** Each shard can have one or more replicas.
** Read / Search operations performed on any of the replica shards.
* Multi Tenant.
** Support for more than one index.
** Index level configuration (number of shards, index storage, ...).
* Various set of APIs
** HTTP RESTful API
** Native Java API.
** All APIs perform automatic node operation rerouting.
* Document oriented
** No need for upfront schema definition.
** Schema can be defined for customization of the indexing process.
* Reliable, Asynchronous Write Behind for long term persistency.
* (Near) Real Time Search.
* Built on top of Lucene
** Each shard is a fully functional Lucene index
** All the power of Lucene easily exposed through simple configuration / plugins.
* Per operation consistency
** Single document level operations are atomic, consistent, isolated and durable.

### Logstash
Logstash is part of the Elastic Stack along with Beats, Elasticsearch and Kibana. Logstash is a server-side data processing pipeline that ingests data from a multitude of sources simultaneously, transforms it, and then sends it to your favorite "stash." (Ours is Elasticsearch, naturally.). Logstash has over 200 plugins, and you can write your own very easily as well.
### Kibana
Kibana is an open source analytics and visualization platform designed to work with Elasticsearch. You use Kibana to search, view, and interact with data stored in Elasticsearch indices. You can easily perform advanced data analysis and visualize your data in a variety of charts, tables, and maps.

Kibana makes it easy to understand large volumes of data. Its simple, browser-based interface enables you to quickly create and share dynamic dashboards that display changes to Elasticsearch queries in real time.

Setting up Kibana is a snap. You can install Kibana and start exploring your Elasticsearch indices in minutes — no code, no additional infrastructure required

### Dependencies
## Installation
Installation commands for ELK on Mac-OS using brew install.

#### Elasticsearch
```
$ brew install elasticsearch
```

```
$ brew services start elasticsearch
$ brew info elasticsearch
```
**Elastic search** is alive, we can get the info with `http://localhost:9200/`
#### Kibana
```
$ brew install kibana
```

```
$ brew services start kibana
$ brew info kibana
```
**Kibana** is alive, we can get the info with `http://localhost:5601/`

#### Logstash
```
$ brew install logstash
```

```
$ brew services start logstash
$ brew info logstash
```

## Presentation 
The work was presented at the Monthly Open Innovation Team Meeting. The slides can be be found [here](https://docs.google.com/presentation/d/1h4iVZrPmYFp3CSzT-wq8gKCAhw2utjlwTCzxDASGgcU/edit?usp=sharing)

## Screenshots
<img src ="https://github.com/akshitac8/diversity_metrics_prototype/blob/master/Prototype-Images/Dashboard.png"></img>

## References
[1][Brief Introduction to Elasticsearch](https://github.com/elastic/elasticsearch)

[2][Brief Introduction to logstash](https://github.com/elastic/logstash)

[3][Brief Introduction to kibana](https://www.elastic.co/guide/en/kibana/current/introduction.html)

[4][Guide to Installation](https://medium.com/@pablo_ezequiel/installing-elk-stack-on-osx-74b132ad1498)

## License
