---
title: Aspose::Cells::Top10 class
linktitle: Top10
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Top10 class. Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified in C++.'
type: docs
weight: 15000
url: /ru/cpp/aspose.cells/top10/
---
## Top10 class


Describe the [Top10](./) conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.

```cpp
class Top10
```

## Methods

| Method | Description |
| --- | --- |
| [GetRank()](./getrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [IsBottom()](./isbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPercent()](./ispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Top10\& src)](./operator_asm/) | operator= |
| [SetIsBottom(bool value)](./setisbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [SetIsPercent(bool value)](./setispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [SetRank(int32_t value)](./setrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [Top10()](./top10/) | Default constructor. |
| [Top10(Top10_Impl* impl)](./top10/) | Constructs from an implementation object. |
| [Top10(const Top10\& src)](./top10/) | Copy constructor. |
| [~Top10()](./~top10/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);

//Добавляет пустое условное форматирование
int index = sheet.GetConditionalFormattings().Add();
FormatConditionCollection fcs = sheet.GetConditionalFormattings().Get(index);

//Устанавливает диапазон условного форматирования.
CellArea ca = CellArea::CreateCellArea(0, 0, 10, 10);
fcs.AddArea(ca);

//Добавляет условие.
int conditionIndex = fcs.AddCondition(FormatConditionType::Top10, OperatorType::None, nullptr, nullptr);
//Устанавливает цвет фона.
FormatCondition fc = fcs.Get(conditionIndex);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });
Top10 top10 = fc.GetTop10();
//Установить Top N
top10.SetRank(5);
//Сохранение файла Excel
workbook.Save(u"output.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
