# canal-adapter
## 基于canal的client-adapter数据同步

本文将介绍canal项目中client-adapter的使用，以及落地生产中需要考虑的可靠性、高可用与监控报警。（基于canal 1.1.5版本）
canal作为mysql的实时数据订阅组件，实现了对mysql binlog数据的抓取。
目前的最新稳定版1.1.5版本中，client-adapter已经实现了同步数据到RDS、ES、HBase、MQ的能力。
