# Changelog

## cp-schema-registry-v7.3.1-bbc-5
* Remove deprecated `UseCGroupMemoryLimitForHeap` which has been replaced by `UseContainerSupport` and is on by default

## cp-schema-registry-v7.3.1-bbc-4
* use bbc-registry image for kafka-prometheus-jmx-exporter

## cp-schema-registry-v7.3.1-bbc-3
* change istio annotations to labels

## cp-schema-registry-v7.3.1-bbc-2

* chore: Upgraded Caddy server to 2.6.4 for the UI
* ref: Standardized configuration with a hard-coded config in the Docker image, no
   entrypoint
* fix: `Oidc_*` Headers are not proxied anymore to the backend Schema
   Registry. This reduces a lot the total header length, avoiding hitting
   the max header length limit on the backend side.
