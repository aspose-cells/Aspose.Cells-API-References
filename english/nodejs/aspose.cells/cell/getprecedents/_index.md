---
title: "Cell.getPrecedents"
linktitle: "getPrecedents"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Gets all references appearing in this cell's formula."
type: docs
weight: 370
url: /nodejs/aspose.cells/cell/getprecedents/
---

## getPrecedents()

Gets all references appearing in this cell's formula. Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.To get those references which influence the calculation only, please use getPrecedentsInCalculation().@return {ReferredAreaCollection} Collection of all references appearing in this cell's formula.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("A1").setFormula("= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1");
var areas = cells.get("A1").getPrecedents();
for (var i = 0; i < areas.getCount(); i++)
{
var area = areas.get(i);
var stringBuilder = "";
if (area.isExternalLink())
{
stringBuilder += "[";
stringBuilder += area.getExternalFileName();
stringBuilder += "]";
}
stringBuilder += area.getSheetName();
stringBuilder += "!";
stringBuilder += aspose.cells.CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn());
if (area.isArea())
{
stringBuilder += ":";
stringBuilder += aspose.cells.CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn());
}
console.log(stringBuilder);
}
workbook.save("Book2.xls");
```
