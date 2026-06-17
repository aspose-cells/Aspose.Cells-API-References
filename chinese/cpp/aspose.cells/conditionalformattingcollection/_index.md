---
title: Aspose::Cells::ConditionalFormattingCollection class
linktitle: ConditionalFormattingCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ConditionalFormattingCollection class. Encapsulates a collection of FormatCondition objects in C++.'
type: docs
weight: 3100
url: /zh/cpp/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class


Encapsulates a collection of [FormatCondition](../formatcondition/) objects.

```cpp
class ConditionalFormattingCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add()](./add/) | Adds a FormatConditions to the collection. |
| [ConditionalFormattingCollection(ConditionalFormattingCollection_Impl* impl)](./conditionalformattingcollection/) | Constructs from an implementation object. |
| [ConditionalFormattingCollection(const ConditionalFormattingCollection\& src)](./conditionalformattingcollection/) | Copy constructor. |
| [Copy(const ConditionalFormattingCollection\& cfs)](./copy/) | Copies conditional formatting. |
| [Get(int32_t index)](./get/) | Gets the FormatConditions element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ConditionalFormattingCollection\& src)](./operator_asm/) | operator= |
| [RemoveArea(int32_t startRow, int32_t startColumn, int32_t totalRows, int32_t totalColumns)](./removearea/) | Remove all conditional formatting in the range. |
| [~ConditionalFormattingCollection()](./~conditionalformattingcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);

//获取条件格式
ConditionalFormattingCollection cformattings = sheet.GetConditionalFormattings();
//添加空的条件格式
int index = cformattings.Add();
//获取新添加的条件格式
FormatConditionCollection fcs = cformattings.Get(index);

//设置条件格式范围。
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);

ca = CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);

//添加条件。
int conditionIndex = fcs.AddCondition(FormatConditionType::CellValue, OperatorType::Between, u"=A2", u"100");
//添加条件。
int conditionIndex2 = fcs.AddCondition(FormatConditionType::CellValue, OperatorType::Between, u"50", u"100");
//设置背景颜色。
FormatCondition fc = fcs.Get(conditionIndex);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });
//保存 Excel 文件
workbook.Save(u"output.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
