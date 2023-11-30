---
title: Aspose::Cells::Workbook::GetStyleInPool method
linktitle: GetStyleInPool
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Workbook::GetStyleInPool method. Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells in C++.'
type: docs
weight: 2300
url: /cpp/aspose.cells/workbook/getstyleinpool/
---
## Workbook::GetStyleInPool method


Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

```cpp
Style Aspose::Cells::Workbook::GetStyleInPool(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index. |

## ReturnValue

The style in the pool corresponds to given index, may be null.
## Remarks



If the returned style is changed, the style of all cells(which refers to this style) will be changed. 
## See Also

* Class [Style](../../style/)
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
