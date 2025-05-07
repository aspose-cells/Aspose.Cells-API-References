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
// Called: if (value.Type == CellValueType.IsError && "#DIV/0!".Equals(value.Value))
public override bool Property_Value(int cellRow, int cellColumn, CellValue value)
            {
                if (value.Type == CellValueType.IsError && "#DIV/0!".Equals(value.Value))
                {
                    value.Type = CellValueType.IsNull;
                    return true;
                }
                return false;
            }
```

### See Also

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


