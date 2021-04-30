# Fix entries for projects that are not Open Source but are listed as such

Some of the projects listed as Open Source with license Other or Unknown do not carry an open source license. These notes are the result of quickly checking each repos license. Please double check before you rely on it. When there are multiple licenses governing a work, the list may only note one of them.

The list is from entries in `processed_landscape.yml` containing `license: Other` or `license: Unknown` as of 3f1e33bd865b3e72a079eed3ab48c2fc689e9d91.

There were some related issues for fixing repos on which Github couldn't detect the license:

https://github.com/cncf/landscape/issues/1061
https://github.com/cncf/landscape/issues/272

The code for the pretty name of these license categories is: https://github.com/cncf/landscapeapp/blob/b26e8cb7238ede044a92a986ce86aa4ed0b62c55/tools/fetchGithubStats.js#L87

The code for marking items as not open source is: https://github.com/cncf/landscapeapp/blob/b26e8cb7238ede044a92a986ce86aa4ed0b62c55/tools/generateJson.js#L165

Repos that need to be fixed by setting open_source: false on the entry, because it doesn't contain an open source licensed version:

Repo URL|License|Notes
-|-|-
https://github.com/cockroachdb/cockroach | BSL
https://github.com/mongodb/mongo | SSPL
https://github.com/dgraph-io/dgraph | custom named
https://github.com/hazelcast/hazelcast | custom named
https://github.com/timescale/timescaledb | custom named
https://github.com/hazelcast/hazelcast-jet | custom named
https://github.com/pachyderm/pachyderm | custom named
https://github.com/getsentry/sentry | BSL
https://github.com/elastic/elasticsearch | SSPL
https://github.com/Graylog2/graylog2-server | SSPL
https://github.com/vectorizedio/redpanda | BSL
https://github.com/stashed/stash | AppsCode
https://github.com/kubedb/operator | AppsCode

Repos that seem to contain an open source licensed version, but Github can't detect it:

Repo URL|License|Notes
-|-|-
https://github.com/cfengine/core | GPL3
https://github.com/digitalrebar/provision | Apache2
https://github.com/maas/maas | AGPL3
https://github.com/inspec/inspec | Apache2
https://github.com/in-toto/in-toto | Apache2
https://github.com/theupdateframework/tuf | Apache2
https://github.com/ceph/ceph | GPL3
https://github.com/gluster/glusterfs | GPL2
https://github.com/open-io/oio-sds | AGPL3
https://github.com/hpcng/singularity | BSD-3-clause
https://github.com/weaveworks/weave | Apache2
https://github.com/OpenNebula/one | Apache2
https://github.com/haproxy/haproxy | GPL2
https://github.com/openresty/openresty | BSD-3-clause
https://github.com/zalando/skipper | MIT
https://github.com/apioak/apioak | Apache2
https://github.com/Kong/kong | Apache2
https://github.com/devopsfaith/krakend | Apache2
https://github.com/mulesoft/mule | CPAL
https://github.com/TykTechnologies/tyk | MPL2
https://github.com/mysql/mysql-server | GPL2
https://github.com/neo4j/neo4j | GPL3
https://github.com/percona/percona-server | GPL2
https://github.com/postgres/postgres | Postgres
https://github.com/tikv/tikv | Apache2
https://github.com/voltdb/voltdb | AGPL3
https://github.com/YugaByte/yugabyte-db | Apache2 +N
https://github.com/apache/storm | Apache2
https://github.com/rabbitmq/rabbitmq-server | MPL2
https://github.com/oam-dev/spec | probably open | [OWF contributor agreement 1.0](http://www.openwebfoundation.org/legal/the-owf-1-0-agreements/owf-contributor-license-agreement-1-0---copyright-and-patent)
https://github.com/drone/drone | Apache2 +N
https://github.com/gitlabhq/gitlabhq | MIT-Expat +N
https://github.com/screwdriver-cd/screwdriver | BSD-3-clause
https://github.com/k0sproject/k0s | Apache2
https://github.com/kubermatic/kubermatic | Apache2 +N
https://github.com/vanillastack/vanillastack | Apache2
https://github.com/akka/akka | Apache2
https://github.com/hasura/graphql-engine | Apache2
https://github.com/Azure/azure-functions-host | MIT
https://github.com/elastic/beats | Apache2 +N
https://github.com/weaveworks/scope | Apache2
https://github.com/elastic/logstash | Apache2 +N
https://github.com/elastic/apm-server | Apache2 +N
https://github.com/joyent/smartos-live | probably open | no repo level license summary and some files are missing a license
https://github.com/nginx/nginx | BSD-2-clause
https://github.com/clearlinux/clr-bundles | probably open | no repo level license summary and some files are missing a license
https://github.com/kubic-project/container-images | probably open | no repo level license summar and some files are missing a license
https://github.com/architect/functions | Apache2
