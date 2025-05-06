---
title: DataSorter.Clear
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Clear all settings
type: docs
url: /net/aspose.cells/datasorter/clear/
---
## DataSorter.Clear method

Clear all settings.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: sorter.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Sort/aTest_20090916_104430_4681099.xlsx&quot;);
            CellArea ca = new CellArea();
            ca.StartRow = 10;
            ca.EndRow = 144;
            ca.StartColumn = 0;
            ca.EndColumn = 7;

            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(4, SortOrder.Ascending);
            sorter.AddKey(6, SortOrder.Ascending);
            sorter.AddKey(7, SortOrder.Ascending);
            sorter.AddKey(5, SortOrder.Ascending);

            sorter.Sort(workbook.Worksheets[&quot;Sheet1&quot;].Cells, ca);

            sorter.Clear();
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;F42&quot;].StringValue, &quot;Single&quot;);
            workbook.Save(Constants.destPath + &quot;Test_199564.xlsx&quot;);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


