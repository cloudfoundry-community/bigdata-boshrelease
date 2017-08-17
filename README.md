# BOSH Release for collection of big data software

Apache Cassandra, Spark, Kafka and Zookeeper

* [Concourse CI](https://ci.starkandwayne.com/teams/main/pipelines/bigdata-boshrelease)
* Pull requests will be automatically tested against a bosh-lite (see `testflight-pr` job)
* Latest upstream project versions are automatically added as blobs via CI
* Discussions and CI notifications at [#bigdata-boshrelease channel](https://cloudfoundry.slack.com/messages/C6R4VJNS2/) on https://slack.cloudfoundry.org

## Usage

To use this BOSH release:

```
export BOSH_ENVIRONMENT=<alias>
export BOSH_DEPLOYMENT=bigdata

git clone https://github.com/cloudfoundry-community/bigdata-boshrelease.git
cd bigdata-boshrelease
bosh2 deploy manifests/bigdata.yml
```
