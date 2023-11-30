---
title: Aspose::Cells::PageSetup::SetHeader method
linktitle: SetHeader
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PageSetup::SetHeader method. Sets a script formatting the header of an Excel file in C++.'
type: docs
weight: 8700
url: /cpp/aspose.cells/pagesetup/setheader/
---
## PageSetup::SetHeader(int32_t, const U16String\&) method


Sets a script formatting the header of an Excel file.

```cpp
void Aspose::Cells::PageSetup::SetHeader(int32_t section, const U16String &headerScript)
```


| Parameter | Type | Description |
| --- | --- | --- |
| section | int32_t | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | const U16String\& | Header format script. |
## Remarks



Script commands:

<table><tr><th>Command </th><th>Description  </th></tr><tr><td>&P </td><td>Current page number　  </td></tr><tr><td>&N </td><td>Page count　  </td></tr><tr><td>&D </td><td>Current date　  </td></tr><tr><td>&T </td><td>Current time  </td></tr><tr><td>&A </td><td>Sheet name  </td></tr><tr><td>&F </td><td>File name without path  </td></tr><tr><td>&"&lt;FontName&gt;" </td><td>Font name, for example: &"Arial"  </td></tr><tr><td>&"&lt;FontName&gt;, &lt;FontStyle&gt;" </td><td>Font name and font style, for example: &"Arial,Bold"  </td></tr><tr><td>&<FontSize> </td><td>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.  </td></tr><tr><td>&K<RRGGBB> </td><td>Font color, for example(RED): &KFF0000  </td></tr><tr><td>&G </td><td>Image script  </td></tr></table>
For example: "&amp;Arial,Bold&amp;8Header Note" 
## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## PageSetup::SetHeader(int32_t, const char16_t*) method


Sets a script formatting the header of an Excel file.

```cpp
void Aspose::Cells::PageSetup::SetHeader(int32_t section, const char16_t *headerScript)
```


| Parameter | Type | Description |
| --- | --- | --- |
| section | int32_t | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | const char16_t* | Header format script. |
## Remarks



Script commands:

<table><tr><th>Command </th><th>Description  </th></tr><tr><td>&P </td><td>Current page number　  </td></tr><tr><td>&N </td><td>Page count　  </td></tr><tr><td>&D </td><td>Current date　  </td></tr><tr><td>&T </td><td>Current time  </td></tr><tr><td>&A </td><td>Sheet name  </td></tr><tr><td>&F </td><td>File name without path  </td></tr><tr><td>&"&lt;FontName&gt;" </td><td>Font name, for example: &"Arial"  </td></tr><tr><td>&"&lt;FontName&gt;, &lt;FontStyle&gt;" </td><td>Font name and font style, for example: &"Arial,Bold"  </td></tr><tr><td>&<FontSize> </td><td>Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.  </td></tr><tr><td>&K<RRGGBB> </td><td>Font color, for example(RED): &KFF0000  </td></tr><tr><td>&G </td><td>Image script  </td></tr></table>
For example: "&amp;Arial,Bold&amp;8Header Note" 
## See Also

* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
