---
title: Aspose::Cells::Drawing::CheckBoxCollection class
linktitle: CheckBoxCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::CheckBoxCollection class. Represents a collection of CheckBox objects in a worksheet in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells.drawing/checkboxcollection/
---
## CheckBoxCollection class


Represents a collection of [CheckBox](../checkbox/) objects in a worksheet.

```cpp
class CheckBoxCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width)](./add/) | Adds a checkBox to the collection. |
| [CheckBoxCollection(CheckBoxCollection_Impl* impl)](./checkboxcollection/) | Constructs from an implementation object. |
| [CheckBoxCollection(const CheckBoxCollection\& src)](./checkboxcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [CheckBox](../checkbox/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CheckBoxCollection\& src)](./operator_asm/) | operator= |
| [~CheckBoxCollection()](./~checkboxcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Create a new Workbook.
Workbook workbook;

//Get the first worksheet in the workbook.
Worksheet sheet = workbook.GetWorksheets().Get(0);

int index = sheet.GetCheckBoxes().Add(15, 15, 20, 100);
CheckBox checkBox = sheet.GetCheckBoxes().Get(index);
checkBox.SetText(u"Check Box 1");


Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
