---
title: ListColumn.TotalsCalculation
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the type of calculation in the Totals row of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Gets and sets the type of calculation in the Totals row of the list column.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Examples

```csharp
// Called: listObject.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;
public void ListColumn_Property_TotalsCalculation()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    Util.SetHintMessage(cells[0, 0], "The file should not be corrupted or in protected view while loading by ms excel");

    cells[1, 0].PutValue("Column A");
    cells[1, 1].PutValue("Column B");
    cells[2, 0].PutValue(1);
    cells[2, 1].PutValue(3);

    ListObject listObject = sheet.ListObjects[sheet.ListObjects.Add(1, 0, 3, 1, true)];
    listObject.TableStyleType = TableStyleType.TableStyleMedium2;
    listObject.DisplayName = "Table";
    //listObject.ListColumns[1].Formula = "=[Column A] + 1";
    listObject.ShowTotals = true;
    listObject.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;
    Util.SaveManCheck(wb, "Formula", "example.xls");
    wb = new Workbook(Constants.checkPath + "example.xls");
    Util.SaveManCheck(wb, "Formula", "example.xlsx");
}
```

### See Also

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


