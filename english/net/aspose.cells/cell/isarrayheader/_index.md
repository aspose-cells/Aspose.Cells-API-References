---
title: Cell.IsArrayHeader
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates the cells formula is an array formula and it is the first cell of the array
type: docs
url: /net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indicates the cell's formula is an array formula and it is the first cell of the array.

```csharp
public bool IsArrayHeader { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["C4"].IsArrayHeader);
[Test]
        public void Property_IsArrayHeader()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41634.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // add 2 rows
            worksheet.Cells.InsertRow(2);
            worksheet.Cells[2, 0].Value = (3);
            worksheet.Cells[2, 1].Value = (4);
            worksheet.Cells.InsertRow(3);
            worksheet.Cells[3, 0].Value = (5);
            worksheet.Cells[3, 1].Value = (6);

            worksheet.ListObjects[0].Resize(0, 0, 3, 2, true);
            workbook.CalculateFormula();

            Assert.IsTrue(worksheet.Cells["C4"].IsArrayHeader);
            workbook.Save(Constants.destPath + "CELLSJAVA41634.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA41634.xlsx");
            Assert.IsTrue(workbook.Worksheets[0].Cells["C4"].IsArrayHeader);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


