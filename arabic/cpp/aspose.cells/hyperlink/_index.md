---
title: Aspose::Cells::Hyperlink class
linktitle: Hyperlink
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Hyperlink class. Encapsulates the object that represents a hyperlink in C++.'
type: docs
weight: 8400
url: /ar/cpp/aspose.cells/hyperlink/
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
//إنشاء كائن Workbook
Workbook workbook;
//إضافة ورقة عمل جديدة إلى كائن Workbook
workbook.GetWorksheets().Add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Adding a hyperlink to a URL at "A1" cell
int index = worksheet.GetHyperlinks().Add(u"A1", 1, 1, u"http://www.aspose.com");
//الحصول على ارتباط تشعبي حسب الفهرس.
Hyperlink hyperlink = worksheet.GetHyperlinks().Get(index);
//تعيين نص العرض لهذا الارتباط التشعبي.
hyperlink.SetTextToDisplay(u"Aspose");
//حفظ ملف Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
