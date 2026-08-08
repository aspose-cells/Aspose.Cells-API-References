---
title: "PivotTableCollection.add"
linktitle: "add"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source."
type: docs
weight: 90
url: /nodejs/aspose.cells/pivottablecollection/add-8/
---

## add(sourceData, isAutoPage, pageFields, destCellName, tableName)

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | Array of String | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |

**Returns:** Number — `Number` The new added PivotTable index.
