---
title: "PivotTableCollection.add"
linktitle: "add"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a new PivotTable cache to a PivotCaches collection."
type: docs
weight: 40
url: /nodejs/aspose.cells/pivottablecollection/add-3/
---

## add(sourceData, row, column, tableName, useSameSource)

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:** Number — `Number` The new added cache index.
