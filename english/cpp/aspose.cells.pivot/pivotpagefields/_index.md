---
title: Aspose::Cells::Pivot::PivotPageFields class
linktitle: PivotPageFields
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotPageFields class. Represents the pivot page items if the pivot table data source is consolidation ranges. It only can contain up to 4 items in C++.'
type: docs
weight: 2100
url: /cpp/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class


Represents the pivot page items if the pivot table data source is consolidation ranges. It only can contain up to 4 items.

```cpp
class PivotPageFields
```

## Methods

| Method | Description |
| --- | --- |
| [AddIdentify(int32_t rangeIndex, const Vector \<int32_t\>\& pageItemIndex)](./addidentify/) | Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first. |
| [AddPageField(const Vector \<U16String\>\& pageItems)](./addpagefield/) | Adds a page field. |
| [GetPageFieldCount()](./getpagefieldcount/) | Gets the number of page fields. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotPageFields\& src)](./operator_asm/) | operator= |
| [PivotPageFields()](./pivotpagefields/) | Represents the pivot page field items. |
| [PivotPageFields(PivotPageFields_Impl* impl)](./pivotpagefields/) | Constructs from an implementation object. |
| [PivotPageFields(const PivotPageFields\& src)](./pivotpagefields/) | Copy constructor. |
| [~PivotPageFields()](./~pivotpagefields/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
