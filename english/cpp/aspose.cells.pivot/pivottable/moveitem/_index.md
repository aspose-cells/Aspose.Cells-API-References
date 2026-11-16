---
title: Aspose::Cells::Pivot::PivotTable::MoveItem method
linktitle: MoveItem
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotTable::MoveItem method. Move one item up or down in C++.'
type: docs
weight: 19400
url: /cpp/aspose.cells.pivot/pivottable/moveitem/
---
## PivotTable::MoveItem method


Move one item up or down.

```cpp
void Aspose::Cells::Pivot::PivotTable::MoveItem(PivotFieldType region, const Vector<U16String> &nodes, bool absolute, int32_t offset)
```


| Parameter | Type | Description |
| --- | --- | --- |
| region | PivotFieldType | The region. Only for row or column. |
| nodes | const Vector \<U16String\>\& | The item. |
| absolute | bool | Indicates whether offset is absolute position. |
| offset | int32_t | If absolute is true :0 move to beginning, -1 move to End, others mean absolute position; else offset is a relative position. |

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotFieldType](../../pivotfieldtype/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
