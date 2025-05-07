---
title: Cell.IsRichText
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Indicates whether the string value of this cell is a rich formatted text
type: docs
url: /net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indicates whether the string value of this cell is a rich formatted text.

```csharp
public bool IsRichText()
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells["B6"].IsRichText(), true);
[Test]
        public void Method_IsRichText()
        {
            string filePath = Constants.sourcePath + "Sort/CELLSNET-42040.xlsx";
            Workbook workbook = new Workbook(filePath);
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 0;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 13;
            ca.EndColumn = 1;
            //Sort data in the specified data range (A1:B14) 
            sorter.Sort(workbook.Worksheets[0].Cells, ca);
            Assert.AreEqual(workbook.Worksheets[0].Cells["B6"].IsRichText(), true);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


