---
title: CellValue.Value
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Gets or sets the cell value
type: docs
url: /net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Gets or sets the cell value.

```csharp
public object Value { get; set; }
```

### Remarks

The value must be of the correct type of object corresponding to the [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null, any other object will be ignored |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | error string such as "#VALUE!", "#NAME?", ... |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### See Also

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


