---
title: Aspose::Cells::Pivot::DiscreteGroupItem class
linktitle: DiscreteGroupItem
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::DiscreteGroupItem class. Represents an item of custom grouped field in C++.'
type: docs
weight: 200
url: /cpp/aspose.cells.pivot/discretegroupitem/
---
## DiscreteGroupItem class


Represents an item of custom grouped field.

```cpp
class DiscreteGroupItem
```

## Methods

| Method | Description |
| --- | --- |
| [DiscreteGroupItem(const U16String\& name, const Vector \<int32_t\>\& itemIndexes)](./discretegroupitem/) | The constructor of custom group item of pivot field. |
| [DiscreteGroupItem(const char16_t* name, const Vector \<int32_t\>\& itemIndexes)](./discretegroupitem/) | The constructor of custom group item of pivot field. |
| [DiscreteGroupItem(const U16String\& name, const Vector \<U16String\>\& items)](./discretegroupitem/) | The constructor of custom group item of pivot field. |
| [DiscreteGroupItem(const char16_t* name, const Vector \<U16String\>\& items)](./discretegroupitem/) | The constructor of custom group item of pivot field. |
| [DiscreteGroupItem(DiscreteGroupItem_Impl* impl)](./discretegroupitem/) | Constructs from an implementation object. |
| [DiscreteGroupItem(const DiscreteGroupItem\& src)](./discretegroupitem/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DiscreteGroupItem\& src)](./operator_asm/) | operator= |
| [~DiscreteGroupItem()](./~discretegroupitem/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"product");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"carrot");
cells.Get(3, 0).PutValue(u"potato");
cells.Get(4, 0).PutValue(u"cherry");

//Create date style
Style dateStyle = CellsFactory().CreateStyle();
dateStyle.SetCustom(u"m/d/yyyy");
cells.Get(0, 1).PutValue(u"date");
cells.Get(1, 1).PutValue(Date{ 2021, 2, 5 });
cells.Get(2, 1).PutValue(Date{ 2022, 3, 8 });
cells.Get(3, 1).PutValue(Date{ 2023, 4, 10 });
cells.Get(4, 1).PutValue(Date{ 2024, 5, 16 });
//Set date style
cells.Get(1, 1).SetStyle(dateStyle);
cells.Get(2, 1).SetStyle(dateStyle);
cells.Get(3, 1).SetStyle(dateStyle);
cells.Get(4, 1).SetStyle(dateStyle);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);

PivotTableCollection pivots = sheet.GetPivotTables();
//Add a PivotTable
PivotTable pivot = pivots.Add(u"=Sheet1!A1:C5", u"A12");

pivot.AddFieldToArea(PivotFieldType::Row, u"product");
pivot.AddFieldToArea(PivotFieldType::Column, u"date");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Group by fruit and vegetable
DiscreteGroupItem fruit(u"fruit", Vector<int>{ 0, 3 });
DiscreteGroupItem vegetable(u"vegetable", Vector<int>{ 1, 2 });
PivotFieldGroupOptions groupOptions;
groupOptions.SetDiscreteGroupItems(Vector<DiscreteGroupItem>{ fruit, vegetable });
pivot.GetRowFields().Get(0).Group(groupOptions);
pivot.CalculateData();


book.Save(u"DiscreteGroup.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
