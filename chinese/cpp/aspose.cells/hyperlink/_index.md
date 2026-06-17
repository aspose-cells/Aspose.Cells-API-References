---
title: Aspose::Cells::Hyperlink class
linktitle: Hyperlink
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Hyperlink class. Encapsulates the object that represents a hyperlink in C++.'
type: docs
weight: 8400
url: /zh/cpp/aspose.cells/hyperlink/
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
//实例化 Workbook 对象
Workbook workbook;
//向 Workbook 对象添加新工作表
workbook.GetWorksheets().Add();
//通过传递工作表索引获取新添加工作表的引用
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//在单元格 "A1" 添加指向 URL 的超链接
int index = worksheet.GetHyperlinks().Add(u"A1", 1, 1, u"http://www.aspose.com");
//通过索引获取超链接。
Hyperlink hyperlink = worksheet.GetHyperlinks().Get(index);
//设置此超链接的显示文本。
hyperlink.SetTextToDisplay(u"Aspose");
//保存 Excel 文件
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
