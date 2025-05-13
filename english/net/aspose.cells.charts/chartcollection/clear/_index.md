---
title: ChartCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Clear all charts
type: docs
url: /net/aspose.cells.charts/chartcollection/clear/
---
## ChartCollection.Clear method

Clear all charts.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: myWorkSheet.Charts.Clear();
public void ChartCollection_Method_Clear()
        {
            Console.WriteLine("ChartCollection_Method_Clear()");
            string infn = path + "TEST_removePivotable.xlsx";
            string outfn = Constants.destPath + "TEST_removePivotable_out.xlsx";
            Workbook book = new Workbook(infn);

            Worksheet myWorkSheet = book.Worksheets["SheetA"];
            myWorkSheet.Cells.DeleteRows(0, myWorkSheet.Cells.MaxRow);
            myWorkSheet.PivotTables.Clear();
            myWorkSheet.Charts.Clear();
            PivotTable pivotTable = myWorkSheet.PivotTables[myWorkSheet.PivotTables.Add("=RawData1All", "A1", "myPivot")];

            book.Save(outfn);
        }
```

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


