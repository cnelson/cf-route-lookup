# Cloud Foundry Route Lookup Plugin

This is a Cloud Foundry CLI plugin to find the application a given hostname/domain/route is bound to. Note this will only show applications in orgs/spaces that the logged-in user has permissions to view.

## Installation

1. Download the appropriate binary from [the Releases page](https://github.com/18F/cf-route-lookup/releases).
1. Run

    ```sh
    cf install-plugin <path/to/cf-route-lookup_*>
    ```

## Usage

```
$ cf lookup-route <my.domain.com>
Bound to:
<org>/<space>/<app>
$ cf lookup-route <unknown.domain.com>
2016/12/12 20:47:10 Error retrieving apps: Route not found.
```
