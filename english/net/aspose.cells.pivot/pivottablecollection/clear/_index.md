---
title: PivotTableCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection method. Clear all pivot tables
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/clear/
---
## PivotTableCollection.Clear method

Clear all pivot tables.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: myWorkSheet.PivotTables.Clear();
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

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


