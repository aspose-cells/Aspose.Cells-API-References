---
title: Aspose::Cells::Pivot::PivotItem class
linktitle: PivotItem
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotItem class. Represents a item in a PivotField report in C++.'
type: docs
weight: 2400
url: /cpp/aspose.cells.pivot/pivotitem/
---
## PivotItem class


Represents a item in a [PivotField](../pivotfield/) report.

```cpp
class PivotItem
```

## Methods

| Method | Description |
| --- | --- |
| [GetDateTimeValue()](./getdatetimevalue/) | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue. |
| [GetDoubleValue()](./getdoublevalue/) | Gets the double value of the pivot item If the value is null or not number ,it will return 0. |
| [GetFormula()](./getformula/) | Gets the formula of this calculated item. Only works when this item is a calculated item. |
| [GetIndex()](./getindex/) |  **(Deprecated)** Gets the index of the pivot item in cache field. |
| [GetName()](./getname/) | Gets the name of the pivot item. |
| [GetPosition()](./getposition/) | Specifying the index of this item in all the PivotItems of the field. |
| [GetPositionInSameParentNode()](./getpositioninsameparentnode/) |  **(Deprecated)** Specifying the position index in the PivotItems under the same parent node. |
| [GetStringValue()](./getstringvalue/) | Gets the string value of the pivot item If the value is null, it will return "". |
| [GetValue()](./getvalue/) | Gets the value of the pivot item. |
| [IsCalculatedItem()](./iscalculateditem/) | Indicates whether this pivot item is a calculated formula item. |
| [IsDetailHidden()](./isdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. |
| [IsHidden()](./ishidden/) | Gets and Sets whether the pivot item is hidden. |
| [IsMissing()](./ismissing/) | Indicates whether the item was removed from the data source. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [Move(int32_t offset, bool isSameParent)](./move/) |  **(Deprecated)** Moves the item up or down. |
| [Move(int32_t offset)](./move/) | Moves the item up or down in the pivot field. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotItem\& src)](./operator_asm/) | operator= |
| [PivotItem(PivotItem_Impl* impl)](./pivotitem/) | Constructs from an implementation object. |
| [PivotItem(const PivotItem\& src)](./pivotitem/) | Copy constructor. |
| [SetIndex(int32_t value)](./setindex/) |  **(Deprecated)** Gets the index of the pivot item in cache field. |
| [SetIsDetailHidden(bool value)](./setisdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. |
| [SetIsHidden(bool value)](./setishidden/) | Gets and Sets whether the pivot item is hidden. |
| [SetName(const U16String\& value)](./setname/) | Gets the name of the pivot item. |
| [SetName(const char16_t* value)](./setname/) | Gets the name of the pivot item. |
| [SetPosition(int32_t value)](./setposition/) | Specifying the index of this item in all the PivotItems of the field. |
| [SetPositionInSameParentNode(int32_t value)](./setpositioninsameparentnode/) |  **(Deprecated)** Specifying the position index in the PivotItems under the same parent node. |
| [~PivotItem()](./~pivotitem/) | Destructor. |
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
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");

cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);

PivotTableCollection pivots = sheet.GetPivotTables();

PivotTable pivot = pivots.Add(u"=Sheet1!A1:C9", u"A12");

pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");

pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Change PivotField's attributes
PivotField rowField = pivot.GetRowFields().Get(0);
rowField.SetDisplayName(u"custom display name");

//Hide the first item
PivotItem item = rowField.GetPivotItems().Get(0);
item.SetIsHidden(true);

pivot.CalculateData();

book.Save(u"out.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
