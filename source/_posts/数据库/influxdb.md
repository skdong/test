# influx demo

influxdb 命令

```bash
influx  -host 3.1.6.61 -port 8086 -username lma -password mNA3DC5QPRUqrRlGNvy17Yh2  -database lma

SELECT mean("value") FROM "cpu_idle" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0)

SELECT mean("value") FROM "cpu_interrupt" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0)
D
SELECT mean("value") FROM "cpu_nice" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0)
E
SELECT mean("value") FROM "cpu_system" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0)
F
SELECT mean("value") FROM "cpu_steal" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0)
G
SELECT mean("value") FROM "cpu_wait" WHERE "hostname" = '$server' AND $timeFilter GROUP BY time($interval) fill(0
 select * from cpu_idle where time > now() - 1m

```


mirantis 监控数据采集服务

```bash
service metric_collector restart
service log_collector restart
collectd

```