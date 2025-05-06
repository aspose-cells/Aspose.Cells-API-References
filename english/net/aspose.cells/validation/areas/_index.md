---
title: Validation.Areas
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Gets all CellArea which contain the data validation settings
type: docs
url: /net/aspose.cells/validation/areas/
---
## Validation.Areas property

Gets all [`CellArea`](../../cellarea/) which contain the data validation settings.

```csharp
public CellArea[] Areas { get; }
```

### Examples

```csharp
// Called: testAreEqual(1, validation.Areas.Length, caseName);
private void Property_Areas(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            testAreEqual(1, sheet.Validations.Count, caseName);
            Validation validation = sheet.Validations[0];
            testAreEqual(1, validation.Areas.Length, caseName);
            CellArea cellarea = (CellArea)validation.Areas[0];
            AssertHelper.checkCellArea(1, 1, 8, 3, cellarea);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


