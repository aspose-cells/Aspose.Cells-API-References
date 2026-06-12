---
title: Aspose::Cells::Hyperlink class
linktitle: Hyperlink
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Hyperlink class. Encapsulates the object that represents a hyperlink in C++.'
type: docs
weight: 8400
url: /sv/cpp/aspose.cells/hyperlink/
---
## Hyperlink class


Encapsulates the object that represents a hyperlink.

```cpp
class Hyperlink
```

## Methods

| Method | Description |
| --- | --- |
| [Delete()](./delete/) | Deletes this hyperlink. |
| [GetAddress()](./getaddress/) | Represents the address of a hyperlink. |
| [GetArea()](./getarea/) | Gets the range of hyperlink. |
| [GetLinkType()](./getlinktype/) | Gets the link type. |
| [GetScreenTip()](./getscreentip/) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [GetTextToDisplay()](./gettexttodisplay/) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [Hyperlink(Hyperlink_Impl* impl)](./hyperlink/) | Constructs from an implementation object. |
| [Hyperlink(const Hyperlink\& src)](./hyperlink/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Hyperlink\& src)](./operator_asm/) | operator= |
| [SetAddress(const U16String\& value)](./setaddress/) | Represents the address of a hyperlink. |
| [SetAddress(const char16_t* value)](./setaddress/) | Represents the address of a hyperlink. |
| [SetScreenTip(const U16String\& value)](./setscreentip/) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [SetScreenTip(const char16_t* value)](./setscreentip/) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [SetTextToDisplay(const U16String\& value)](./settexttodisplay/) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [SetTextToDisplay(const char16_t* value)](./settexttodisplay/) | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [~Hyperlink()](./~hyperlink/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;
//Lägger till ett nytt kalkylblad till Workbook-objektet
workbook.GetWorksheets().Add();
//Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Lägger till en hyperlänk till en URL i cellen "A1"
int index = worksheet.GetHyperlinks().Add(u"A1", 1, 1, u"http://www.aspose.com");
//Hämtar en hyperlänk efter index.
Hyperlink hyperlink = worksheet.GetHyperlinks().Get(index);
//Ställer in visningstext för denna hyperlänk.
hyperlink.SetTextToDisplay(u"Aspose");
//Sparar Excel-filen
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
