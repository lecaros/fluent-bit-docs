# Table of contents

* [Fluent Bit v1.8 Documentation](README.md)

## About

* [What is Fluent Bit ?](about/what-is-fluent-bit.md)
* [A Brief History of Fluent Bit](about/history.md)
* [Fluentd & Fluent Bit](about/fluentd-and-fluent-bit.md)
* [License](about/license.md)

## Concepts

* [Key Concepts](concepts/key-concepts.md)
* [Buffering](concepts/buffering.md)
* [Data Pipeline](concepts/data-pipeline/README.md)
  * [Input](concepts/data-pipeline/input.md)
  * [Parser](concepts/data-pipeline/parser.md)
  * [Filter](concepts/data-pipeline/filter.md)
  * [Buffer](concepts/data-pipeline/buffer.md)
  * [Router](concepts/data-pipeline/router.md)
  * [Output](concepts/data-pipeline/output.md)

## Installation

* [Getting Started with Fluent Bit](installation/getting-started-with-fluent-bit.md)
* [Upgrade Notes](installation/upgrade-notes.md)
* [Supported Platforms](installation/supported-platforms.md)
* [Requirements](installation/requirements.md)
* [Sources](installation/sources/README.md)
  * [Download Source Code](installation/sources/download-source-code.md)
  * [Build and Install](installation/sources/build-and-install.md)
  * [Build with Static Configuration](installation/sources/build-with-static-configuration.md)
* [Linux Packages](installation/linux/README.md)
  * [Amazon Linux](installation/linux/amazon-linux.md)
  * [Redhat / CentOS](installation/linux/redhat-centos.md)
  * [Debian](installation/linux/debian.md)
  * [Ubuntu](installation/linux/ubuntu.md)
  * [Raspbian / Raspberry Pi](installation/linux/raspbian-raspberry-pi.md)
* [Docker](installation/docker.md)
* [Containers on AWS](installation/aws-container.md)
* [Amazon EC2](installation/amazon-ec2.md)
* [Kubernetes](installation/kubernetes.md)
* [Yocto / Embedded Linux](installation/yocto-embedded-linux.md)
* [Windows](installation/windows.md)

## Administration

* [Configuring Fluent Bit](administration/configuring-fluent-bit/README.md)
  * [Format and Schema](administration/configuring-fluent-bit/format-schema.md)
  * [Configuration File](administration/configuring-fluent-bit/configuration-file.md)
  * [Variables](administration/configuring-fluent-bit/variables.md)
  * [Commands](administration/configuring-fluent-bit/commands.md)
  * [Upstream Servers](administration/configuring-fluent-bit/upstream-servers.md)
  * [Unit Sizes](administration/configuring-fluent-bit/unit-sizes.md)
  * [Multiline Parsing](administration/configuring-fluent-bit/multiline-parsing.md)
  * [Record Accessor](administration/configuring-fluent-bit/record-accessor.md)
* [Security](administration/security.md)
* [Buffering & Storage](administration/buffering-and-storage.md)
* [Backpressure](administration/backpressure.md)
* [Scheduling and Retries](administration/scheduling-and-retries.md)
* [Networking](administration/networking.md)
* [Memory Management](administration/memory-management.md)
* [Monitoring](administration/monitoring.md)
* [Dump Internals / Signal](administration/dump-internals-signal.md)
* [HTTP Proxy](administration/http-proxy.md)

## Local Testing

* [Validating your Data and Structure](local-testing/validating-your-data-and-structure.md)
* [Running a Logging Pipeline Locally](local-testing/logging-pipeline.md)

## Data Pipeline <a id="pipeline"></a>

* [Pipeline Monitoring](pipeline/pipeline-monitoring.md)
* [Inputs](pipeline/inputs/README.md)
  * [Node Exporter Metrics](pipeline/inputs/node-exporter-metrics.md)
  * [Collectd](pipeline/inputs/collectd.md)
  * [CPU Metrics](pipeline/inputs/cpu-metrics.md)
  * [Disk I/O Metrics](pipeline/inputs/disk-io-metrics.md)
  * [Docker Metrics](pipeline/inputs/docker-metrics.md)
  * [Docker Events](pipeline/inputs/docker-events.md)
  * [Dummy](pipeline/inputs/dummy.md)
  * [Exec](pipeline/inputs/exec.md)
  * [Forward](pipeline/inputs/forward.md)
  * [Head](pipeline/inputs/head.md)
  * [HTTP](pipeline/inputs/http.md)
  * [Health](pipeline/inputs/health.md)
  * [Kernel Logs](pipeline/inputs/kernel-logs.md)
  * [Memory Metrics](pipeline/inputs/memory-metrics.md)
  * [MQTT](pipeline/inputs/mqtt.md)
  * [Network I/O Metrics](pipeline/inputs/network-io-metrics.md)
  * [Process Metrics](pipeline/inputs/process.md)
  * [Random](pipeline/inputs/random.md)
  * [Serial Interface](pipeline/inputs/serial-interface.md)
  * [Standard Input](pipeline/inputs/standard-input.md)
  * [StatsD](pipeline/inputs/statsd.md)
  * [Syslog](pipeline/inputs/syslog.md)
  * [Systemd](pipeline/inputs/systemd.md)
  * [Tail](pipeline/inputs/tail.md)
  * [TCP](pipeline/inputs/tcp.md)
  * [Thermal](pipeline/inputs/thermal.md)
  * [Windows Event Log](pipeline/inputs/windows-event-log.md)
* [Parsers](pipeline/parsers/README.md)
  * [Configuring Parser](pipeline/parsers/configuring-parser.md)
  * [JSON](pipeline/parsers/json.md)
  * [Regular Expression](pipeline/parsers/regular-expression.md)
  * [LTSV](pipeline/parsers/ltsv.md)
  * [Logfmt](pipeline/parsers/logfmt.md)
  * [Decoders](pipeline/parsers/decoders.md)
* [Filters](pipeline/filters/README.md)
  * [AWS Metadata](pipeline/filters/aws-metadata.md)
  * [CheckList](pipeline/filters/checklist.md)
  * [Expect](pipeline/filters/expect.md)
  * [GeoIP2 Filter](pipeline/filters/geoip2-filter.md)
  * [Grep](pipeline/filters/grep.md)
  * [Kubernetes](pipeline/filters/kubernetes.md)
  * [Lua](pipeline/filters/lua.md)
  * [Parser](pipeline/filters/parser.md)
  * [Record Modifier](pipeline/filters/record-modifier.md)
  * [Modify](pipeline/filters/modify.md)
  * [Multiline](pipeline/filters/multiline-stacktrace.md)
  * [Nest](pipeline/filters/nest.md)
  * [Rewrite Tag](pipeline/filters/rewrite-tag.md)
  * [Standard Output](pipeline/filters/standard-output.md)
  * [Throttle](pipeline/filters/throttle.md)
  * [Tensorflow](pipeline/filters/tensorflow.md)
* [Outputs](pipeline/outputs/README.md)
  * [Prometheus Exporter](pipeline/outputs/prometheus-exporter.md)
  * [Prometheus Remote Write](pipeline/outputs/prometheus-remote-write.md)
  * [Amazon CloudWatch](pipeline/outputs/cloudwatch.md)
  * [Amazon Kinesis Data Firehose](pipeline/outputs/firehose.md)
  * [Amazon Kinesis Data Streams](pipeline/outputs/kinesis.md)
  * [Amazon S3](pipeline/outputs/s3.md)
  * [Azure Log Analytics](pipeline/outputs/azure.md)
  * [Azure Blob](pipeline/outputs/azure_blob.md)
  * [Google Cloud BigQuery](pipeline/outputs/bigquery.md)
  * [Counter](pipeline/outputs/counter.md)
  * [Datadog](pipeline/outputs/datadog.md)
  * [Elasticsearch](pipeline/outputs/elasticsearch.md)
  * [File](pipeline/outputs/file.md)
  * [FlowCounter](pipeline/outputs/flowcounter.md)
  * [Forward](pipeline/outputs/forward.md)
  * [GELF](pipeline/outputs/gelf.md)
  * [HTTP](pipeline/outputs/http.md)
  * [InfluxDB](pipeline/outputs/influxdb.md)
  * [Kafka](pipeline/outputs/kafka.md)
  * [Kafka REST Proxy](pipeline/outputs/kafka-rest-proxy.md)
  * [LogDNA](pipeline/outputs/logdna.md)
  * [Loki](pipeline/outputs/loki.md)
  * [NATS](pipeline/outputs/nats.md)
  * [New Relic](pipeline/outputs/new-relic.md)
  * [NULL](pipeline/outputs/null.md)
  * [PostgreSQL](pipeline/outputs/postgresql.md)
  * [Slack](pipeline/outputs/slack.md)
  * [Stackdriver](pipeline/outputs/stackdriver.md)
  * [Standard Output](pipeline/outputs/standard-output.md)
  * [Splunk](pipeline/outputs/splunk.md)
  * [Syslog](pipeline/outputs/syslog.md)
  * [TCP & TLS](pipeline/outputs/tcp-and-tls.md)
  * [Treasure Data](pipeline/outputs/treasure-data.md)
  * [WebSocket](pipeline/outputs/websocket.md)

## Stream Processing

* [Introduction to Stream Processing](stream-processing/introduction.md)
* [Overview](stream-processing/overview.md)
* [Changelog](stream-processing/changelog.md)
* [Getting Started](stream-processing/getting-started/README.md)
  * [Fluent Bit + SQL](stream-processing/getting-started/fluent-bit-sql.md)
  * [Check Keys and NULL values](stream-processing/getting-started/check-keys-null-values.md)
  * [Hands On! 101](stream-processing/getting-started/hands-on.md)

## Fluent Bit for Developers <a id="development"></a>

* [C Library API](development/library_api.md)
* [Ingest Records Manually](development/ingest-records-manually.md)
* [Golang Output Plugins](development/golang-output-plugins.md)
* [Developer guide for beginners on contributing to Fluent Bit](development/developer-guide.md)

