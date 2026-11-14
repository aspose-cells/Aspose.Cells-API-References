---
title: Aspose::Cells::Pivot::PivotShowValuesSetting class
linktitle: PivotShowValuesSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotShowValuesSetting class. Represents the settings about showing values as when the ShowDataAs calculation is in use in C++.'
type: docs
weight: 2900
url: /cpp/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class


Represents the settings about showing values as when the ShowDataAs calculation is in use.

```cpp
class PivotShowValuesSetting
```

## Methods

| Method | Description |
| --- | --- |
| [GetBaseFieldIndex()](./getbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [GetBaseFieldName()](./getbasefieldname/) | Gets caption of the pivot base field. |
| [GetBaseItemCaption()](./getbaseitemcaption/) | Gets caption of the pivot item in the base field. |
| [GetBaseItemIndex()](./getbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [GetBaseItemPositionType()](./getbaseitempositiontype/) |  **(Deprecated)** Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [GetCalculationType()](./getcalculationtype/) |  **(Deprecated)** Represents how to show values of a data field in the pivot report. |
| [GetShowValuesAs()](./getshowvaluesas/) | Gets and sets how to show values of a data field in the pivot report. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotShowValuesSetting\& src)](./operator_asm/) | operator= |
| [PivotShowValuesSetting(PivotShowValuesSetting_Impl* impl)](./pivotshowvaluessetting/) | Constructs from an implementation object. |
| [PivotShowValuesSetting(const PivotShowValuesSetting\& src)](./pivotshowvaluessetting/) | Copy constructor. |
| [SetBaseFieldIndex(int32_t value)](./setbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [SetBaseItemIndex(int32_t value)](./setbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [SetBaseItemPositionType(PivotItemPositionType value)](./setbaseitempositiontype/) |  **(Deprecated)** Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [SetCalculationType(PivotFieldDataDisplayFormat value)](./setcalculationtype/) |  **(Deprecated)** Represents how to show values of a data field in the pivot report. |
| [SetShowValuesAs(PivotShowValuesAsType value)](./setshowvaluesas/) | Gets and sets how to show values of a data field in the pivot report. |
| [~PivotShowValuesSetting()](./~pivotshowvaluessetting/) | Destructor. |
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

PivotField dataField = pivot.GetDataFields().Get(0);
// Display value as percentage of the grand total
//dataField.ShowValuesAs(PivotShowValuesAsType::PercentageOfTotal, 0, PivotShowValuesSetting.NextPivotItem);
// Get the display calculation setting of data field
PivotShowValuesSetting settings = dataField.GetShowValuesSetting();
//std::cout << settings.GetShowValuesAs() <<std::endl;

pivot.CalculateData();

book.Save(u"out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
