# StatsD backend for StatsD

## Overview
This is a pluggable backend for [StatsD](https://github.com/etsy/statsd), which
publishes stats to another StatsD service.

## Installation
  
    TBD

## Configuration
Here is some more elaborate example: runs the statsd server locally on 
127.0.0.100:8125 which will flush every 5 seconds via UDP to the central
statsd on 192.169.111.11:8125

```
{
  statsdHost: '192.169.111.11'
, statsdPort: 8125
, statsdDebug: false
, flushInterval: 10000
, backends: ["statsd-backend"]
, debug: false
, debugInterval: 5000
, address: '127.0.0.100'
, port: 8125
}
```

## Dependencies
- [statsd-client](https://github.com/msiebuhr/node-statsd-client)

## Development
- [Bugs](https://github.com/dynmeth/statsd-backend/issues)
