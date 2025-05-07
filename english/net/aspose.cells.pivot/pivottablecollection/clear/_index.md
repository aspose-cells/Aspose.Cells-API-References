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
            Console.WriteLine("Method_Clear()");
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

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


