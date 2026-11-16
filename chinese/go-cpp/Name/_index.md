---
title: "Name 类"
linktitle: "Name"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Name 类。封装在 Go 中表示 name 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/name/
---

## Name class

表示对单元格范围的已定义名称。

```go

type Name struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetComment](./getcomment/) | 获取和设置名称的注释。仅适用于 Excel 2007 或更高版本。 |
| [SetComment](./setcomment/) | 获取和设置名称的注释。仅适用于 Excel 2007 或更高版本。 |
| [GetText](./gettext/) | 获取对象的名称文本。 |
| [SetText](./settext/) | 获取对象的名称文本。 |
| [GetFullText](./getfulltext/) | 获取对象在范围设置下的名称完整文本。 |
| [GetRefersTo](./getrefersto/) | 返回或设置该名称定义引用的公式，以等号开头。 |
| [SetRefersTo_String](./setrefersto_string/) | 返回或设置该名称定义引用的公式，以等号开头。 |
| [GetR1C1RefersTo](./getr1c1refersto/) | 获取或设置该名称的 R1C1 引用。 |
| [SetR1C1RefersTo](./setr1c1refersto/) | 获取或设置该名称的 R1C1 引用。 |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | 获取此名称的引用。 |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | 根据指定单元格获取此名称的引用。 |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | 设置此名称的引用。 |
| [IsReferred](./isreferred/) | 指示此名称是否被其他公式引用。 |
| [IsVisible](./isvisible/) | 指示该名称是否可见。 |
| [SetIsVisible](./setisvisible/) | 指示该名称是否可见。 |
| [GetSheetIndex](./getsheetindex/) | 指示此名称属于工作簿还是工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。 |
| [SetSheetIndex](./setsheetindex/) | 指示此名称属于工作簿还是工作表。0 = 全局名称，否则为工作表索引（从 1 开始）。 |
| [ToString](./tostring/) | 返回表示当前 Range 对象的字符串。 |
| [GetRanges](./getranges/) | 获取此名称引用的所有范围。 |
| [GetRanges_Bool](./getranges_bool/) | 获取此名称引用的所有范围。 |
| [GetReferredAreas](./getreferredareas/) | 获取此名称引用的所有引用。 |
| [GetRange](./getrange/) | 如果此名称引用的是范围，则获取该范围。 |
| [GetRange_Bool](./getrange_bool/) | 如果此名称引用的是范围，则获取该范围 |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | 如果此名称引用的是范围，则获取该范围。如果此名称的引用不是绝对的，则在不同单元格时范围可能不同。 |
