---
title: Aspose::Cells::AutoFilter class
linktitle: AutoFilter
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::AutoFilter class. Represents autofiltering for the specified worksheet in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells/autofilter/
---
## AutoFilter class


Represents autofiltering for the specified worksheet.

```cpp
class AutoFilter
```

## Methods

| Method | Description |
| --- | --- |
| [AddDateFilter(int32_t fieldIndex, DateTimeGroupingType dateTimeGroupingType, int32_t year, int32_t month, int32_t day, int32_t hour, int32_t minute, int32_t second)](./adddatefilter/) | Adds a date filter. |
| [AddFillColorFilter(int32_t fieldIndex, BackgroundType pattern, const CellsColor\& foregroundColor, const CellsColor\& backgroundColor)](./addfillcolorfilter/) | Adds a fill color filter. |
| [AddFilter(int32_t fieldIndex, const U16String\& criteria)](./addfilter/) | Adds a filter for a filter column. |
| [AddFilter(int32_t fieldIndex, const char16_t* criteria)](./addfilter/) | Adds a filter for a filter column. |
| [AddFontColorFilter(int32_t fieldIndex, const CellsColor\& color)](./addfontcolorfilter/) | Adds a font color filter. |
| [AddIconFilter(int32_t fieldIndex, IconSetType iconSetType, int32_t iconId)](./addiconfilter/) | Adds an icon filter. |
| [AutoFilter(AutoFilter_Impl* impl)](./autofilter/) | Constructs from an implementation object. |
| [AutoFilter(const AutoFilter\& src)](./autofilter/) | Copy constructor. |
| [Custom(int32_t fieldIndex, FilterOperatorType operatorType1, const Aspose::Cells::Object\& criteria1)](./custom/) | Filters a list with a custom criterion. |
| [Custom(int32_t fieldIndex, FilterOperatorType operatorType1, const Aspose::Cells::Object\& criteria1, bool isAnd, FilterOperatorType operatorType2, const Aspose::Cells::Object\& criteria2)](./custom/) | Filters a list with custom criteria. |
| [Dynamic_Filter(int32_t fieldIndex, DynamicFilterType dynamicFilterType)](./dynamic_filter/) | Adds a dynamic filter. |
| [Filter(int32_t fieldIndex, const U16String\& criteria)](./filter/) | Filters a list with specified criteria. |
| [Filter(int32_t fieldIndex, const char16_t* criteria)](./filter/) | Filters a list with specified criteria. |
| [FilterTop10(int32_t fieldIndex, bool isTop, bool isPercent, int32_t itemCount)](./filtertop10/) | Filter the top 10 items in the list. |
| [GetCellArea()](./getcellarea/) | Gets the [CellArea](../cellarea/) where the this [AutoFilter](./) applies to. |
| [GetCellArea(bool refreshAppliedRange)](./getcellarea/) | Gets the [Aspose.Cells.CellArea](../cellarea/) where the specified [AutoFilter](./) applies. |
| [GetFilterColumns()](./getfiltercolumns/) | Gets the collection of the filter columns. |
| [GetRange()](./getrange/) | Represents the range to which the specified [AutoFilter](./) applies. |
| [GetShowFilterButton()](./getshowfilterbutton/) | Indicates whether the [AutoFilter](./) button for this column is visible. |
| [GetSorter()](./getsorter/) | Gets the data sorter. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [MatchBlanks(int32_t fieldIndex)](./matchblanks/) | Match all blank cells in the list. |
| [MatchNonBlanks(int32_t fieldIndex)](./matchnonblanks/) | Match all not-blank cells in the list. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AutoFilter\& src)](./operator_asm/) | operator= |
| [Refresh()](./refresh/) | Refresh auto filters to hide or unhide the rows. |
| [Refresh(bool hideRows)](./refresh/) | Gets all hidden rows' indexes. |
| [RemoveDateFilter(int32_t fieldIndex, DateTimeGroupingType dateTimeGroupingType, int32_t year, int32_t month, int32_t day, int32_t hour, int32_t minute, int32_t second)](./removedatefilter/) | Removes a date filter. |
| [RemoveFilter(int32_t fieldIndex, const U16String\& criteria)](./removefilter/) | Removes a filter for a filter column. |
| [RemoveFilter(int32_t fieldIndex, const char16_t* criteria)](./removefilter/) | Removes a filter for a filter column. |
| [RemoveFilter(int32_t fieldIndex)](./removefilter/) | Remove the specific filter. |
| [SetRange(int32_t row, int32_t startColumn, int32_t endColumn)](./setrange/) | Sets the range to which the specified [AutoFilter](./) applies. |
| [SetRange(const U16String\& value)](./setrange/) | Represents the range to which the specified [AutoFilter](./) applies. |
| [SetRange(const char16_t* value)](./setrange/) | Represents the range to which the specified [AutoFilter](./) applies. |
| [SetShowFilterButton(bool value)](./setshowfilterbutton/) | Indicates whether the [AutoFilter](./) button for this column is visible. |
| [ShowAll()](./showall/) | Unhide all rows. |
| [~AutoFilter()](./~autofilter/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Creating a file stream containing the Excel file to be opened
//Instantiating a Workbook object
Workbook workbook(u"template.xlsx");
//Accessing the first worksheet in the Excel file
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Creating AutoFilter by giving the cells range of the heading row
worksheet.GetAutoFilter().SetRange(u"A1:B1");
//Filtering columns with specified values
worksheet.GetAutoFilter().Filter(1, u"Bananas");
//Saving the modified Excel file.
workbook.Save(u"output.xls");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
