---
title: Impala所有端口
date: 2022-03-03 20:37:47
tags: [Impala]
categories:
- 工作
top: 0
toc: false
copyright: true
---

##### Impala所有端口

<!--more-->

|       Scope / Role       |         Startup Flag          | Default Port |                           Comment                            |
| :----------------------: | :---------------------------: | :----------: | :----------------------------------------------------------: |
|      Impala Daemon       |        --beeswax_port         |    21000     | Port on which Beeswax client requests are served by Impala Daemons. |
|      Impala Daemon       |          --hs2_port           |    21050     | Port on which HiveServer2 client requests are served by Impala Daemons. |
|      Impala Daemon       |           --be_port           |    22000     | Internal use only. Impala daemons use this port for Thrift based communication with each other. |
|      Impala Daemon       | --state_store_subscriber_port |    23000     | Internal use only. Impala daemons listen on this port for updates from the StateStore daemon. |
|      Catalog Daemon      | --state_store_subscriber_port |    23020     | Internal use only. The Catalog Server daemon listens on this port for updates from the StateStore daemon. |
|      Impala Daemon       |       --webserver_port        |    25000     | Impala debug Web UI for administrators to monitor and troubleshoot. |
| Impala StateStore Daemon |       --webserver_port        |    25010     | StateStore debug Web UI for administrators to monitor and troubleshoot. |
|  Impala Catalog Daemon   |       --webserver_port        |    25020     | Catalog Server debug Web UI for administrators to monitor and troubleshoot. New in Impala 1.2 and higher. |
| Impala StateStore Daemon |      --state_store_port       |    24000     | Internal use only. The StateStore daemon listens on this port for registration/unregistration requests. |
|  Impala Catalog Daemon   |    --catalog_service_port     |    26000     | Internal use only. The Catalog Server uses this port to communicate with the Impala daemons. New in Impala 1.2 and higher. |
|      Impala Daemon       |          --krpc_port          |    27000     | Internal use only. Impala daemons use this port for KRPC based communication with each other. |
|      Impala Daemon       |        --hs2_http_port        |    28000     | Used to transmit commands and receive results by client applications over HTTP via the HiveServer2 protocol. |

