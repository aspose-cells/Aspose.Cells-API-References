---
title: Validation.GetListValue
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Get the value for list of the validation for the specified cell
type: docs
url: /net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Get the value for list of the validation for the specified cell.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [`ReferredArea`](../../referredarea/) object; Otherwise the returned value may be null, object[], or simple object.

### Remarks

Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


