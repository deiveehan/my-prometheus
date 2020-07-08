

#### metric name
metric name refers to the attribute being measured. 
- probably returns multiple data points. 

#### metric label
- labels are used to provide dimensional data model. 

![](.readme_images/13c08998.png)

metric name can have more than one labels.

#### Queriying
You can use the metric name / label to query / filter results. 

![](.readme_images/462001a5.png)


### Metric types

#### Counter
- a number that can only increase or set to zero. 

```text
node_cpu_seconds_total[5m]
```

#### Guage
- single number that can increase or decrease over time. 
- Example, current cpu usage now, no. of http request, memory usage, active threads. 

```text
node_memory_MemAvailable_bytes[5m]
```
![](.readme_images/d7e5b872.png)

#### Histogram
- represents series of data. 
- has _sum & _count
```
prometheus_http_request_duration_seconds_sum{handler="/metrics"}
prometheus_http_request_duration_seconds_count{handler="/metrics"}
```
![](.readme_images/d4c60a8b.png)

#### Summary
- represent data in terms of a quantile (similar to percentile)

![](.readme_images/5021f6b6.png)

