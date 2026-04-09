---
title: Aspose::Cells::Range::Intersect method
linktitle: Intersect
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::Intersect method. Returns a Range object that represents the rectangular intersection of two ranges in C++.'
type: docs
weight: 1200
url: /zh/cpp/aspose.cells/range/intersect/
---
## Range::Intersect method


Returns a [Range](../) object that represents the rectangular intersection of two ranges.

```cpp
Range Aspose::Cells::Range::Intersect(const Range &range)
```


| Parameter | Type | Description |
| --- | --- | --- |
| range | const Range\& | The intersecting range. |

## ReturnValue

Returns a [Range](../) object
## Remarks



If the two ranges are not intersected, returns null.

## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
// 获取第一个工作表的单元格。
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Range range1 = cells.CreateRange(u"A1:A5");
Range range2 = cells.CreateRange(u"A3:A10");
//获取两个范围的交叉范围。
Range intersectRange = range1.Intersect(range2);
//保存 Excel 文件
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Range](../)
* Class [Vector](../../vector/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
