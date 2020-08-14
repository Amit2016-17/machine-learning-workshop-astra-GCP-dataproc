![DataStax Logo](./jupyter/images/DS-logo-2020-White-Blue.png)
# Machine Learning with Apache Spark & Cassandra
## Spark + Cassandra = :heart:
## Spark + DataStax Astra = :fire: :rocket: :stars:

#### A hands-on workshop delivered by DataStax's Developer Advocates team. 
Want to learn about the awesomness of distributed databases and computational systems?
Want to get hands-on with DataStax's Cassandra-as-a-Service offering (_for free!_) and use popular Machine Learning tools and algorithms?
Join in and follow along with this workshop!

## Requirements

* [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [DataStax Astra Registration](http://astra.datastax.com) (_sign up with the email you used to register for the workshop!_)
* [gcloud SDK](https://cloud.google.com/sdk/docs#install_the_latest_cloud_tools_version_cloudsdk_current_version)
* [GCP dataproc](https://console.cloud.google.com/dataproc/clusters)
* [GCS bucket](https://console.cloud.google.com/storage)

## Installation

```
git clone https://github.com/ajgoade/machine-learning-workshop-astra-GCP-dataproc.git
cd machine-learning-workshop-astra-online
gcloud sync <your

```

## Setup

- Download the [Secure Connect Bundle](https://docs.datastax.com/en/astra/aws/doc/dscloud/astra/dscloudObtainingCredentials.html) for your Astra Database
- Move the Secure Connect Bundle to [./jupyter/secureconnect](./jupyter/secureconnect)  
- For the Cassandra lab, access [DataStax Developer Studio on Astra](https://docs.datastax.com/en/astra/aws/doc/dscloud/astra/dscloudConnectStudio.html)
- For the Spark labs, access Jupyter Notebooks: http://localhost:8888 password: `datastax`

You may need to use some custom IP instead of `localhost` if you use docker-for-mac, docker-for-windows or similar installation.

## Known Issues

In some cases executing the exercises may lead to memory issues, especially on weaker or non-Linux machines due to docker limitations on memory. If you have any issues with exercises after the first few, try to clean up and start again `docker-compose kill && docker-compose down && docker-compose up -d`. You may need to repeat steps of the notebook you were working on.
