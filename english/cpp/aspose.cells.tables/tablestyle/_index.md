---
title: Aspose::Cells::Tables::TableStyle class
linktitle: TableStyle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Tables::TableStyle class. Represents the style of the table in C++.'
type: docs
weight: 500
url: /cpp/aspose.cells.tables/tablestyle/
---
## TableStyle class


Represents the style of the table.

```cpp
class TableStyle
```

## Methods

| Method | Description |
| --- | --- |
| [GetName()](./getname/) | Gets the name of table style. |
| [GetTableStyleElements()](./gettablestyleelements/) | Gets all elements of the table style. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TableStyle\& src)](./operator_asm/) | operator= |
| [TableStyle(TableStyle_Impl* impl)](./tablestyle/) | Constructs from an implementation object. |
| [TableStyle(const TableStyle\& src)](./tablestyle/) | Copy constructor. |
| [~TableStyle()](./~tablestyle/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook;
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.SetPattern(BackgroundType::Solid);
firstColumnStyle.SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });//Red

Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.GetFont().SetIsBold(true);
lastColumnStyle.SetPattern(BackgroundType::Solid);
lastColumnStyle.SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });//Red
U16String tableStyleName = u"Custom1";
TableStyleCollection tableStyles = workbook.GetWorksheets().GetTableStyles();
int index1 = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles.Get(index1);
TableStyleElementCollection elements = tableStyle.GetTableStyleElements();
index1 = elements.Add(TableStyleElementType::FirstColumn);
TableStyleElement element = elements.Get(index1);
element.SetElementStyle(firstColumnStyle);
index1 = elements.Add(TableStyleElementType::LastColumn);
element = elements.Get(index1);
element.SetElementStyle(lastColumnStyle);
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
for (int i = 0; i < 5; i++)
{
    cells.Get(0, i).PutValue(CellsHelper::ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
    for (int column = 0; column < 5; column++)
    {
        cells.Get(row, column).PutValue(row * column);
    }
}
ListObjectCollection tables = workbook.GetWorksheets().Get(0).GetListObjects();
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables.Get(0);
table.SetShowTableStyleFirstColumn(true);
table.SetShowTableStyleLastColumn(true);
table.SetTableStyleName(tableStyleName);
workbook.Save(u"Book1.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Tables](../)
* Library [Aspose.Cells for C++](../../)
