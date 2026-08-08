---
title: "Worksheet.xmlMapQuery"
linktitle: "xmlMapQuery"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Query cell areas that mapped/linked to the specific path of xml map."
type: docs
weight: 1480
url: /nodejs/aspose.cells/worksheet/xmlmapquery/
---

## xmlMapQuery(path, xmlMap)

Query cell areas that mapped/linked to the specific path of xml map. e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To query "Attribute1", path is "/RootElement/@Attribute1" To query "Attribute2", path is "/RootElement/SubElement/@Attribute2" To query whole "SubElement", path is "/RootElement/SubElement"

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | xml element path |
| xmlMap | XmlMap | Specify an xml map if you want to query for the specific path within a specific map |

**Returns:** ArrayList — `ArrayList` CellArea list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.
