---
title: DataSorter.HasHeaders
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents whether the range has headers
type: docs
url: /net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Represents whether the range has headers.

```csharp
public bool HasHeaders { get; set; }
```

### Examples

```csharp
// Called: sorter.HasHeaders = true;
[Test]
        public void Property_HasHeaders()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Sort/File_for_CustomSort_ASPOSE_Forum_Question.xlsx&quot;);
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, &quot;aaa,ddd,ccc,bbb&quot;);
            sorter.HasHeaders = true;
            sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea(&quot;A1&quot;, &quot;C23&quot;));
            Cells cells = workbook.Worksheets[1].Cells;
            Assert.AreEqual(cells[&quot;A2&quot;].StringValue, &quot;aaa&quot;);
            Assert.AreEqual(cells[&quot;A7&quot;].StringValue, &quot;ddd&quot;);
            Assert.AreEqual(cells[&quot;A12&quot;].StringValue, &quot;ccc&quot;);
            Assert.AreEqual(cells[&quot;A18&quot;].StringValue, &quot;bbb&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET42150.xlsx&quot;);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


