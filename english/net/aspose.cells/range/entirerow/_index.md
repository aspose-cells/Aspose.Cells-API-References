---
title: Range.EntireRow
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets a Range object that represents the entire row or rows that contains the specified range
type: docs
url: /net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Gets a Range object that represents the entire row (or rows) that contains the specified range.

```csharp
public Range EntireRow { get; }
```

### Examples

```csharp
// Called: var cutRange = sheet.Cells.CreateRange(&amp;quot;A1&amp;quot;).EntireRow;
[Test]
        public void Property_EntireRow()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet47581.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[&quot;Sheet1&quot;];

            var oldMaxCol = sheet.Cells.MaxColumn;

            var cutRange = sheet.Cells.CreateRange(&quot;A1&quot;).EntireRow;
            var pasteRange = sheet.Cells.CreateRange(&quot;A4&quot;).EntireRow;

            sheet.Cells.InsertCutCells(
                cutRange: cutRange,
                row: pasteRange.FirstRow,
                column: pasteRange.FirstColumn,
                shiftType: ShiftType.Down);

            var newMaxCol = sheet.Cells.MaxColumn;

            Assert.AreEqual(newMaxCol, oldMaxCol);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


