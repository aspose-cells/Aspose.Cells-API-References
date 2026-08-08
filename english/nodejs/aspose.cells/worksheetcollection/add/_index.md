---
title: "WorksheetCollection.add"
linktitle: "add"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Adds a worksheet to the collection."
type: docs
weight: 10
url: /nodejs/aspose.cells/worksheetcollection/add/
---

## add(type)

Adds a worksheet to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | SheetType |

**Returns:** Number — `Number` Worksheet object index.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
workbook.getWorksheets().add(aspose.cells.SheetType.CHART);
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("c2").putValue(5000);
cells.get("c3").putValue(3000);
cells.get("c4").putValue(4000);
cells.get("c5").putValue(5000);
cells.get("c6").putValue(6000);
var charts = workbook.getWorksheets().get(1).getCharts();
var chartIndex = charts.add(aspose.cells.ChartType.COLUMN, 10, 10, 20, 20);
var chart = charts.get(chartIndex);
chart.getNSeries().add("Sheet1!C2:C6", true);
```
