---
title: Aspose::Cells::HorizontalPageBreak class
linktitle: HorizontalPageBreak
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::HorizontalPageBreak class. Encapsulates the object that represents a horizontal page break in C++.'
type: docs
weight: 7800
url: /tr/cpp/aspose.cells/horizontalpagebreak/
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
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;

//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Y30 hücresine bir sayfa sonu ekle
int Index = worksheet.GetHorizontalPageBreaks().Add(u"Y30");

//Yeni eklenen yatay sayfa sonunu al
HorizontalPageBreak hPageBreak = worksheet.GetHorizontalPageBreaks().Get(Index);

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
