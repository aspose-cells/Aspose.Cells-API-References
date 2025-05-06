---
title: CellValue.Value
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Gets/sets the cell value
type: docs
url: /net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Gets/sets the cell value.

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
// Called: cell.PutValue(cellValue.Value);
public static void Property_Value()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a CellValue instance
            CellValue cellValue = new CellValue();

            // Set the type and value of the cell
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Assign the CellValue to a cell in the worksheet
            Cell cell = worksheet.Cells[&quot;A1&quot;];
            cell.PutValue(cellValue.Value);

            // Save the workbook
            workbook.Save(&quot;CellValueExample.xlsx&quot;);
            workbook.Save(&quot;CellValueExample.pdf&quot;);
            return;
        }
```

### See Also

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


