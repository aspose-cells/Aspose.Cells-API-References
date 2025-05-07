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
// Called: var cutRange = sheet.Cells.CreateRange("A1").EntireRow;
[Test]
        public void Property_EntireRow()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet47581.xlsx");
            Worksheet sheet = wb.Worksheets["Sheet1"];

            var oldMaxCol = sheet.Cells.MaxColumn;

            var cutRange = sheet.Cells.CreateRange("A1").EntireRow;
            var pasteRange = sheet.Cells.CreateRange("A4").EntireRow;

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


