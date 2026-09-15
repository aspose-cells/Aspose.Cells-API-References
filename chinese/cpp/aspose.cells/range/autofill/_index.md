---
title: Aspose::Cells::Range::AutoFill method
linktitle: AutoFill
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::AutoFill method. Automaticall fill the target range in C++.'
type: docs
weight: 600
url: /zh/cpp/aspose.cells/range/autofill/
---
## Range::AutoFill(const Range\&) method


Automaticall fill the target range.

```cpp
void Aspose::Cells::Range::AutoFill(const Range &target)
```


| Parameter | Type | Description |
| --- | --- | --- |
| target | const Range\& | the target range. |


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
// 获取第一个工作表的单元格。
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").PutValue(1);
cells.Get(u"A2").PutValue(2);
Range source = cells.CreateRange(u"A1:A2");
Range targetRange = cells.CreateRange(u"A3:A10");
//将 3,4,5....10 填充到范围 A3:A10
source.AutoFill(targetRange);
//保存 Excel 文件
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [Range](../)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Range::AutoFill(const Range\&, AutoFillType) method


Automaticall fill the target range.

```cpp
void Aspose::Cells::Range::AutoFill(const Range &target, AutoFillType autoFillType)
```


| Parameter | Type | Description |
| --- | --- | --- |
| target | const Range\& | The targed range. |
| autoFillType | AutoFillType | The auto fill type. |

## See Also

* Class [Vector](../../vector/)
* Class [Range](../)
* Enum [AutoFillType](../../autofilltype/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
