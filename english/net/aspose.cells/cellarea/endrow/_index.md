---
title: CellArea.EndRow
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end row of this area
type: docs
url: /net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Gets or set the end row of this area.

```csharp
public int EndRow;
```

### Examples

```csharp
// Called: EndRow = processingRange.FirstRow + (processingRange.RowCount - 1),
[Test]
        public void Field_EndRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CellsNet46916.xlsb");
            Aspose.Cells.Range processingRange = workbook.Worksheets.GetRangeByName("abc");

            var startColumn = GetCellArea(processingRange).StartColumn;
            var columnIndexToBePopulated = startColumn + 1;

            for (int i = columnIndexToBePopulated; i < 100; i++)
            {
                CellArea rangeArea = new CellArea
                {
                    StartRow = processingRange.FirstRow,
                    StartColumn = i,
                    EndRow = processingRange.FirstRow + (processingRange.RowCount - 1),
                    EndColumn = i
                };

                processingRange.Worksheet.Cells.InsertRange(rangeArea, 1, ShiftType.Right, true);
                // processingRange.Worksheet.Cells.InsertColumn(i);
            }

            workbook.Save(Constants.destPath + "CellsNet46916.xlsx");
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


