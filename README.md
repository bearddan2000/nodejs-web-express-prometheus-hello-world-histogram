# nodejs-web-express-prometheus-hello-world-histogram

## Description
Another way to serve web content.
Uses prometheus to duration of http calls.

To see a graph of visitors:
- Nav to http://localhost:81
- Classic UI
  - Click Graph tab
    - Search: 'scrape_series_added'
      or 'scrape_duration_second'
      or 'http_request_duration_ms_bucket'
    - Duration 1m

For health check:
- Nav to http://localhost:81
- Targetes

## Tech stack
- nodejs
- prometheus

## Docker stack
- node:latest
- prom/prometheus:latest

## To run
`sudo ./install.sh -u`
- Available http://localhost
- App metrics http://localhost/metrics
- Prometheus console http://localhost:81

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- https://dev.to/farnabaz/monitor-your-application-with-prometheus-2886
- https://github.com/RisingStack/example-prometheus-nodejs/blob/master/src/server.js
