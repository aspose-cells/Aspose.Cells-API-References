---
title: Worksheet.GetSelectedAreas
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Gets selected ranges of cells in the designer spreadsheet
type: docs
url: /net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Gets selected ranges of cells in the designer spreadsheet.

```csharp
public Range[] GetSelectedAreas()
```

### Return Value

Returns all selected ranges.

### Examples

```csharp
// Called: rs = workbook.Worksheets[0].GetSelectedAreas();
[Test]
        public void Method_GetSelectedAreas()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SRange01.xlsx");
            Aspose.Cells.Range[] rs = workbook.Worksheets[0].GetSelectedAreas();
            Assert.AreEqual(2, rs.Length);
            workbook.Worksheets[0].SelectRange(1, 1, 2, 2, true);
            rs = workbook.Worksheets[0].GetSelectedAreas();
            Assert.AreEqual(1, rs.Length);
        }
```

### See Also

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


