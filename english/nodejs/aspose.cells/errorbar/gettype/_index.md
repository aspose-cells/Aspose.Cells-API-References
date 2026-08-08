---
title: "ErrorBar.getType"
linktitle: "getType"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents error bar amount type."
type: docs
weight: 220
url: /nodejs/aspose.cells/errorbar/gettype/
---

## getType()

Represents error bar amount type. The value of the property is ErrorBarType integer constant.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("a1").putValue(2);
cells.get("a2").putValue(5);
cells.get("a3").putValue(3);
cells.get("a4").putValue(6);
cells.get("b1").putValue(4);
cells.get("b2").putValue(3);
cells.get("b3").putValue(6);
cells.get("b4").putValue(7);
cells.get("C1").putValue("Q1");
cells.get("C2").putValue("Q2");
cells.get("C3").putValue("Y1");
cells.get("C4").putValue("Y2");
var chartIndex = workbook.getWorksheets().get(0).getCharts().add(aspose.cells.ChartType.COLUMN, 11, 0, 27, 10);
var chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
chart.getNSeries().add("A1:B4", true);
chart.getNSeries().setCategoryData("C1:C4");
for (var i = 0; i < chart.getNSeries().getCount(); i++)
{
var aseries = chart.getNSeries().get(i);
//Sets custom error bar type
aseries.getXErrorBar().setType(aspose.cells.ErrorBarType.CUSTOM);
aseries.getXErrorBar().setPlusValue("=Sheet1!A1");
aseries.getXErrorBar().setMinusValue("=Sheet1!A2");
}
```
