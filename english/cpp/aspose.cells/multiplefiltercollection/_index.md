---
title: Aspose::Cells::MultipleFilterCollection class
linktitle: MultipleFilterCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::MultipleFilterCollection class. Represents the multiple filter collection in C++.'
type: docs
weight: 10700
url: /cpp/aspose.cells/multiplefiltercollection/
---
## MultipleFilterCollection class


Represents the multiple filter collection.


>Deprecated
>
>Use FilterColumn.FilterValueCollection, instead. 
```cpp
class MultipleFilterCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const U16String\& filter)](./add/) | Adds a label filter criteria. |
| [Add(const char16_t* filter)](./add/) | Adds a label filter criteria. |
| [Add(DateTimeGroupingType type, int32_t year, int32_t month, int32_t day)](./add/) | Adds a date filter criteria value. |
| [Add(DateTimeGroupingType type, int32_t year, int32_t month, int32_t day, int32_t hour, int32_t minute, int32_t second)](./add/) | Adds a date time filter criteria value. |
| [begin()](./begin/) | Returns an iterator to the beginning of the [MultipleFilterCollection](./). |
| [end()](./end/) | Returns an iterator to the end of the [MultipleFilterCollection](./). |
| [Get(int32_t index)](./get/) | Gets [DateTimeGroupItem](../datetimegroupitem/) or a string value. |
| [GetCount()](./getcount/) | Gets the count of the filter values. |
| [GetEnumerator()](./getenumerator/) | Get the enumerator for filter value,. |
| [GetMatchBlank()](./getmatchblank/) | Indicates whether to filter by blank. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [MultipleFilterCollection()](./multiplefiltercollection/) |  **(Deprecated)** Constructs one new instance. |
| [MultipleFilterCollection(MultipleFilterCollection_Impl* impl)](./multiplefiltercollection/) | Constructs from an implementation object. |
| [MultipleFilterCollection(const Aspose::Cells::Object\& obj)](./multiplefiltercollection/) | Constructs from an [Object](../object/) convertible to this. |
| [MultipleFilterCollection(const MultipleFilterCollection\& src)](./multiplefiltercollection/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const MultipleFilterCollection\& src)](./operator_asm/) | operator= |
| [SetMatchBlank(bool value)](./setmatchblank/) | Indicates whether to filter by blank. |
| [ToObject()](./toobject/) | Gets the [Object](../object/). |
| [~MultipleFilterCollection()](./~multiplefiltercollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


NOTE: This class is now obsolete. Instead,please use [FilterValueCollection](../filtervaluecollection/) instead. This property will be removed 12 months later since June 2026. **Aspose** apologizes for any inconvenience you may have experienced.


## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
