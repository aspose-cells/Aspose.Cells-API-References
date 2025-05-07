---
title: Cells.IsColumnHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a column at given index is hidden
type: docs
url: /net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Checks whether a column at given index is hidden.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index |

### Return Value

true if the column is hidden.

### Examples

```csharp
// Called: Assert.AreEqual(sheet.Cells.IsColumnHidden(1), true);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet40351.xlsx");
            AutoFitterOptions options = new AutoFitterOptions();
            options.IgnoreHidden = true;
            Worksheet sheet = workbook.Worksheets[0];
            sheet.AutoFitColumns(options);
            Assert.AreEqual(sheet.Cells.IsColumnHidden(1), true);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


