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
// Called: var columnDRange = workbook.Worksheets[&amp;quot;Sheet1&amp;quot;].Cells.CreateRange(1, 3, 1, 1).EntireColumn;
[Test]
        public void Property_EntireColumn()
        {
            var workbook = new Workbook(Constants.sourcePath + @&quot;CELLSNET47205.xlsx&quot;);
            var columnDRange = workbook.Worksheets[&quot;Sheet1&quot;].Cells.CreateRange(1, 3, 1, 1).EntireColumn;
            var style = columnDRange[0, 0].GetStyle();
            style.Custom = &quot;##0%&quot;;
            var styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            columnDRange.ApplyStyle(style, styleFlag);
            Assert.AreEqual(788,workbook.Worksheets[&quot;Sheet1&quot;].Cells.MaxRow);
            workbook.Save(Constants.destPath + &quot;CELLSNET47205.xlsx&quot;);

        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


