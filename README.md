# ELK日志收集系统上线需要解决的问题

## ES
 1. es的集群不能自动发现
 2. es的analysis是否自动开启
 3. es索引的命名，是自动，还是一个服务指定固定一个名字。
 4. es的类型名，如何指定。

## Logstash
 1. 时间戳格式，是否默认，以及替换。是否清除某些无用数据
 2. nginx等程序可以输出JSON格式，加快处理速度，降低消耗，看是否要如此解决。
 3. agent是不是新增一个监控项，就开一个agent。还是一个服务器上只开一个，当有新项目可以监控时，修改配置文件，再启动。
 4. redis输出可能是个瓶颈。开启多个DB应该无法解决，将来的解决方案可能是增加redis.
 5. 

## Zabbix
 1. 统一意见，实时输出还是定时脚本。
 2. 确定监控项
