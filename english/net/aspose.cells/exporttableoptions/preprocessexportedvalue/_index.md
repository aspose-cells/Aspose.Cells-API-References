---
title: ExportTableOptions.PreprocessExportedValue
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions method. Preprocess the value of current cell to be exported
type: docs
url: /net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Preprocess the value of current cell to be exported.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellRow | Int32 | the row index of current cell |
| cellColumn | Int32 | the column index of cell |
| value | CellValue | value and type of current cell |

### Return Value

Whether current cell has been replaced with different type and/or value.

### Remarks

The row and column index is cell's absolute index in the worksheet, not index in the exported table. User may check the value of current cell in the override implementation of this method, if current cell needs to be replaced with other type and value, here the implementation should set the expected type and value to the CellValue object and return true. By default this method does nothing and returns false.

### See Also

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


