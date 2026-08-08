---
title: "Cells.linkToXmlMap"
linktitle: "linkToXmlMap"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Link to a xml map."
type: docs
weight: 1410
url: /nodejs/aspose.cells/cells/linktoxmlmap/
---

## linkToXmlMap(mapName, row, column, path)

Link to a xml map. e.g. A xml map element structure: -RootElement |-Attribute1 |-SubElement |-Attribute2 |-Attribute3 To link "Attribute1", path is "/RootElement/Attribute1" To link "Attribute2", path is "/RootElement/SubElement/Attribute2" To link whole "SubElement", path is "/RootElement/SubElement"

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Number | row of the destination cell |
| column | Number | column of the destination cell |
| path | String | path of xml element in xml map |
