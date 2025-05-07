---
title: Range.EntireColumn
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets a Range object that represents the entire column or columns that contains the specified range
type: docs
url: /net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Gets a Range object that represents the entire column (or columns) that contains the specified range.

```csharp
public Range EntireColumn { get; }
```

### Examples

```csharp
// Called: var columnDRange = workbook.Worksheets["Sheet1"].Cells.CreateRange(1, 3, 1, 1).EntireColumn;
[Test]
        public void Property_EntireColumn()
        {
            var workbook = new Workbook(Constants.sourcePath + @"CELLSNET47205.xlsx");
            var columnDRange = workbook.Worksheets["Sheet1"].Cells.CreateRange(1, 3, 1, 1).EntireColumn;
            var style = columnDRange[0, 0].GetStyle();
            style.Custom = "##0%";
            var styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            columnDRange.ApplyStyle(style, styleFlag);
            Assert.AreEqual(788,workbook.Worksheets["Sheet1"].Cells.MaxRow);
            workbook.Save(Constants.destPath + "CELLSNET47205.xlsx");

        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


