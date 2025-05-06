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
public void Method_Clear()
        {
            Console.WriteLine(&quot;Method_Clear()&quot;);
            string infn = path + &quot;TEST_removePivotable.xlsx&quot;;
            string outfn = Constants.destPath + &quot;TEST_removePivotable_out.xlsx&quot;;
            Workbook book = new Workbook(infn);

            Worksheet myWorkSheet = book.Worksheets[&quot;SheetA&quot;];
            myWorkSheet.Cells.DeleteRows(0, myWorkSheet.Cells.MaxRow);
            myWorkSheet.PivotTables.Clear();
            myWorkSheet.Charts.Clear();
            PivotTable pivotTable = myWorkSheet.PivotTables[myWorkSheet.PivotTables.Add(&quot;=RawData1All&quot;, &quot;A1&quot;, &quot;myPivot&quot;)];

            book.Save(outfn);
        }
```

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


