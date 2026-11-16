---
title: "BuiltInDocumentPropertyCollection 类"
linktitle: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "BuiltInDocumentPropertyCollection 类。封装在 Go 中表示 builtindocumentpropertycollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/builtindocumentpropertycollection/
---

## BuiltInDocumentPropertyCollection class

内置文档属性的集合。

```go

type BuiltInDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewBuiltInDocumentPropertyCollection](./newbuiltindocumentpropertycollection/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Get_String](./get_string/) | 通过属性名称返回 DocumentProperty 对象。 |
| [Get_Int](./get_int/) | 通过索引返回 DocumentProperty 对象。 |
| [GetLanguage](./getlanguage/) | 获取或设置文档的语言。 |
| [SetLanguage](./setlanguage/) | 获取或设置文档的语言。 |
| [GetAuthor](./getauthor/) | 获取或设置文档作者的姓名。 |
| [SetAuthor](./setauthor/) | 获取或设置文档作者的姓名。 |
| [GetComments](./getcomments/) | 获取或设置文档注释。 |
| [SetComments](./setcomments/) | 获取或设置文档注释。 |
| [GetCategory](./getcategory/) | 获取或设置文档的类别。 |
| [SetCategory](./setcategory/) | 获取或设置文档的类别。 |
| [GetContentType](./getcontenttype/) | 获取或设置文档的内容类型。 |
| [SetContentType](./setcontenttype/) | 获取或设置文档的内容类型。 |
| [GetContentStatus](./getcontentstatus/) | 获取或设置文档的内容状态。 |
| [SetContentStatus](./setcontentstatus/) | 获取或设置文档的内容状态。 |
| [GetCompany](./getcompany/) | 获取或设置公司属性。 |
| [SetCompany](./setcompany/) | 获取或设置公司属性。 |
| [GetHyperlinkBase](./gethyperlinkbase/) | 获取或设置 hyperlinkbase 属性。 |
| [SetHyperlinkBase](./sethyperlinkbase/) | 获取或设置 hyperlinkbase 属性。 |
| [GetCreatedTime](./getcreatedtime/) | 获取或设置文档创建日期（本地时区）。 |
| [SetCreatedTime](./setcreatedtime/) | 获取或设置文档创建日期（本地时区）。 |
| [GetCreatedUniversalTime](./getcreateduniversaltime/) | 获取或设置文档创建的 UTC 时间。 |
| [SetCreatedUniversalTime](./setcreateduniversaltime/) | 获取或设置文档创建的 UTC 时间。 |
| [GetKeywords](./getkeywords/) | 获取或设置文档关键字。 |
| [SetKeywords](./setkeywords/) | 获取或设置文档关键字。 |
| [GetLastPrinted](./getlastprinted/) | 获取或设置文档上次打印的日期（本地时区）。 |
| [SetLastPrinted](./setlastprinted/) | 获取或设置文档上次打印的日期（本地时区）。 |
| [GetLastPrintedUniversalTime](./getlastprinteduniversaltime/) | 获取或设置文档上次打印的 UTC 时间。 |
| [SetLastPrintedUniversalTime](./setlastprinteduniversaltime/) | 获取或设置文档上次打印的 UTC 时间。 |
| [GetLastSavedBy](./getlastsavedby/) | 获取或设置最后一位作者的姓名。 |
| [SetLastSavedBy](./setlastsavedby/) | 获取或设置最后一位作者的姓名。 |
| [GetLastSavedTime](./getlastsavedtime/) | 获取或设置最后保存的时间（本地时区）。 |
| [SetLastSavedTime](./setlastsavedtime/) | 获取或设置最后保存的时间（本地时区）。 |
| [GetLastSavedUniversalTime](./getlastsaveduniversaltime/) | 获取或设置最后保存的 UTC 时间。 |
| [SetLastSavedUniversalTime](./setlastsaveduniversaltime/) | 获取或设置最后保存的 UTC 时间。 |
| [GetManager](./getmanager/) | 获取或设置经理属性。 |
| [SetManager](./setmanager/) | 获取或设置经理属性。 |
| [GetNameOfApplication](./getnameofapplication/) | 获取或设置应用程序的名称。 |
| [SetNameOfApplication](./setnameofapplication/) | 获取或设置应用程序的名称。 |
| [GetPages](./getpages/) | 表示对文档页数的估计。 |
| [SetPages](./setpages/) | 表示对文档页数的估计。 |
| [GetRevisionNumber](./getrevisionnumber/) | 获取或设置文档的修订号。 |
| [SetRevisionNumber](./setrevisionnumber/) | 获取或设置文档的修订号。 |
| [GetSubject](./getsubject/) | 获取或设置文档的主题。 |
| [SetSubject](./setsubject/) | 获取或设置文档的主题。 |
| [GetTemplate](./gettemplate/) | 获取或设置文档模板的说明性名称。 |
| [SetTemplate](./settemplate/) | 获取或设置文档模板的说明性名称。 |
| [GetTitle](./gettitle/) | 获取或设置文档的标题。 |
| [SetTitle](./settitle/) | 获取或设置文档的标题。 |
| [GetTotalEditingTime](./gettotaleditingtime/) | 获取或设置总编辑时间（分钟）。 |
| [SetTotalEditingTime](./settotaleditingtime/) | 获取或设置总编辑时间（分钟）。 |
| [GetVersion](./getversion/) | 表示创建文档的应用程序的版本号。 |
| [SetVersion](./setversion/) | 表示创建文档的应用程序的版本号。 |
| [GetDocumentVersion](./getdocumentversion/) | 表示文件的版本。 |
| [SetDocumentVersion](./setdocumentversion/) | 表示文件的版本。 |
| [GetScaleCrop](./getscalecrop/) | 指示文档缩略图的显示模式。 |
| [SetScaleCrop](./setscalecrop/) | 指示文档缩略图的显示模式。 |
| [GetLinksUpToDate](./getlinksuptodate/) | 指示文档中的超链接是否是最新的。 |
| [SetLinksUpToDate](./setlinksuptodate/) | 指示文档中的超链接是否是最新的。 |
| [GetWords](./getwords/) | 表示对文档字数的估计。 |
| [SetWords](./setwords/) | 表示对文档字数的估计。 |
| [Contains](./contains/) | 如果集合中存在具有指定名称的属性，则返回 true。 |
| [IndexOf](./indexof/) | 通过名称获取属性的索引。 |
| [Remove](./remove/) | 从集合中删除具有指定名称的属性。 |
| [RemoveAt](./removeat/) | 删除指定索引处的属性。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
