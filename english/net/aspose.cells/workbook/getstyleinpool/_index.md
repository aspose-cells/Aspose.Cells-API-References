---
title: Workbook.GetStyleInPool
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells
type: docs
url: /net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

```csharp
public Style GetStyleInPool(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |

### Return Value

The style in the pool corresponds to given index, may be null.

### Remarks

If the returned style is changed, the style of all cells(which refers to this style) will be changed.

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


