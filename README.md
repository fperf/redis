# Benchmark Redis

This is a client of [fperf](https://github.com/shafreeck/fperf) which benchmarks Redis

## How to use

### Build fperf with redis support
```
go get github.com/shafreeck/fperf/bin/fperf-build
go get github.com/fperf/redis
fperf-build github.com/fperf/redis
```

### Run the benchmark

```
./fperf -connection 128 -server redis://localhost:6379 redis set key:__rand_int__ "hello fperf"
```
