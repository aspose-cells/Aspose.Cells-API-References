---
title: Aspose::Cells::HorizontalPageBreak class
linktitle: HorizontalPageBreak
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HorizontalPageBreak class. Encapsulates the object that represents a horizontal page break in C++.'
type: docs
weight: 7800
url: /sv/cpp/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class


Encapsulates the object that represents a horizontal page break.

```cpp
class HorizontalPageBreak
```

## Methods

| Method | Description |
| --- | --- |
| [GetEndColumn()](./getendcolumn/) | Gets the end column index of this horizontal page break. |
| [GetRow()](./getrow/) | Gets the zero based row index. |
| [GetStartColumn()](./getstartcolumn/) | Gets the start column index of this horizontal page break. |
| [HorizontalPageBreak(HorizontalPageBreak_Impl* impl)](./horizontalpagebreak/) | Constructs from an implementation object. |
| [HorizontalPageBreak(const HorizontalPageBreak\& src)](./horizontalpagebreak/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const HorizontalPageBreak\& src)](./operator_asm/) | operator= |
| [~HorizontalPageBreak()](./~horizontalpagebreak/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;

//Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Lägg till en sidbrytning vid cell Y30
int Index = worksheet.GetHorizontalPageBreaks().Add(u"Y30");

//hämta den nyligen tillagda horisontella sidbrytningen
HorizontalPageBreak hPageBreak = worksheet.GetHorizontalPageBreaks().Get(Index);

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
