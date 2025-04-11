---
title: Aspose::Cells::LowCode::HtmlConverter class
linktitle: HtmlConverter
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::LowCode::HtmlConverter class. Converter for conversion between html files(html or mht) and other spreadsheet file formats in C++.'
type: docs
weight: 400
url: /cpp/aspose.cells.lowcode/htmlconverter/
---
## HtmlConverter class


Converter for conversion between html files(html or mht) and other spreadsheet file formats.

```cpp
class HtmlConverter
```

## Methods

| Method | Description |
| --- | --- |
| [HtmlConverter(HtmlConverter_Impl* impl)](./htmlconverter/) | Constructs from an implementation object. |
| [HtmlConverter(const HtmlConverter\& src)](./htmlconverter/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const HtmlConverter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts given template file between html and other formats. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts given template file between html and other formats. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts file between html and other spreadsheet file formats. |
| [~HtmlConverter()](./~htmlconverter/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
HtmlConverter::Process(u"Template.xlsx", u"res.html");
```

## See Also

* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
