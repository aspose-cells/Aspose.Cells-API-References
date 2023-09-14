---
title: CellValue.Value
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Represents the cell value
type: docs
url: /net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Represents the cell value.

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

### See Also

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


