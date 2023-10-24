# GeoViz: A Multi-View Visual Platform for Spatio-temporal Knowledge Graph
## Overview

We propose a *Tree-Net-Map* multi-view visualization method to assist in analyzing STKG. Specifically, we have customized three visualization modes for STKG, namely *knowledge tree*, *knowledge net*, and *knowledge map*. Our approach not only reflects the rich attributes and relationships between knowledge triplets, but also highlights the inherent spatio-temporal characteristics of knowledge triplets from three distinct perspectives. For the convenience of users, we have developed a one-stop platform called **GeoViz** to support customized visualization needs with an easy-to-use web user interface. The high level system design of our GeoViz is shown in Figure. Demo visitors can explore our services via https://mdkg.acemap.cn/.

## How to use GeoViz?

### Workflow

![workflow](https://github.com/JeremyChou28/GeoViz/blob/main/workflow.jpg)

Figure 1 shows the workflow of our platform.

1. Access the homepage (A) of our platform through the web user interface, which consists of two parts: visualization and knowledge discovery.
2. Upload users’ spatio-temporal knowledge graph data based on customized service requirements, and then define relevant settings (B) for the back-end to parse the received data.
3. After successful completion of the preceding steps, users can receive a link to access visualization results of three distinct modes: the knowledge tree (C1), the knowledge net (C2), and the knowledge map (C3).
4. Choose the knowledge discovery part (D1), which utilizes the pre-defined prompt in the back-end to discover novel knowledge links from existing data (D2).

### Demo

**Demo data**

Users can upload their own spatio-temporal knowledge graph (STKG) data to complete their customization needs.

Here we give a demo data for case study.

`demo_data/node_data.csv` is the entity data in STKG.

`demo_data/edge_data.csv` is the relationship data between entities in STKG.

We apply the User System to protect user data. Here, we provide a set of username and password for testing.

Username: `geoviztest`

Password: `geoviztest`

**Demo video**



## Discussion

|                        Tools                        | Tree-Net-Map(multi-view) | ST Filter | ST Interaction | Knowledge Discovery | Open Source |
| :-------------------------------------------------: | :----------------------: | :-------: | :------------: | :-----------------: | :---------: |
|             [D3.js](https://d3js.org/)              |            ×             |     ×     |       ×        |          ×          |      √      |
|            [Vis.js](https://visjs.org/)             |            ×             |     ×     |       ×        |          ×          |      √      |
| [Echarts](https://echarts.apache.org/zh/index.html) |            ×             |     ×     |       ×        |          ×          |      √      |
|       [Antv G6](https://antv-g6.gitee.io/zh/)       |            ×             |     ×     |       ×        |          ×          |      √      |
|        [Neo4j(Database)](https://neo4j.com/)        |            ×             |     √     |       √        |          ×          |      √      |
|        **[GeoViz](https://mdkg.acemap.cn/)**        |            √             |     √     |       √        |          √          |      √      |

**GeoViz** is the first concentrated on *Tree-Net-Map* multi-view visual platform for STKG. Moreover, **GeoViz** has spatio-temporal
filters(ST Filter) and supports dynamic spatio-temporal interactions(ST Interaction). In addition, **GeoViz** also provides the function of autonomous knowledge discovery. Although Neo4j provides a web user interface for knowledge graph visualization, it requires interaction through the *Cypher* programming language, which is unfriendly to users. Last but not least, **GeoViz**, like mainstream visualization tools, is open-source.