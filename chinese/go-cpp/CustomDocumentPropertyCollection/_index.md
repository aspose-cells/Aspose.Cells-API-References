---
title: "CustomDocumentPropertyCollection 类"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CustomDocumentPropertyCollection 类。封装了在 Go 中表示 customdocumentpropertycollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

自定义文档属性的集合。

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Add_String_String](./add_string_string/) | 创建一个新的自定义文档属性，数据类型为 <b>PropertyType.String</b>。 |
| [Add_String_Int](./add_string_int/) | 创建一个新的自定义文档属性，数据类型为 <b>PropertyType.Number</b>。 |
| [Add_String_Date](./add_string_date/) | 创建一个新的自定义文档属性，数据类型为 <b>PropertyType.DateTime</b>。 |
| [Add_String_Bool](./add_string_bool/) | 创建一个新的自定义文档属性，数据类型为 <b>PropertyType.Boolean</b>。 |
| [Add_String_Double](./add_string_double/) | 创建一个新的自定义文档属性，数据类型为 <b>PropertyType.Float</b>。 |
| [AddLinkToContent](./addlinktocontent/) | 创建一个链接到内容的自定义文档属性。 |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | 更新所有链接到内容的自定义属性的值（使用 usecell 的链接范围值来更新自定义属性的值）。 |
| [UpdateLinkedRange](./updatelinkedrange/) | 更新所有链接到自定义属性的范围（使用自定义文档属性的值来更新链接范围的单元格值）。 |
| [Get_Int](./get_int/) | 通过索引返回 DocumentProperty 对象。 |
| [Contains](./contains/) | 如果集合中存在具有指定名称的属性，则返回 true。 |
| [IndexOf](./indexof/) | 通过名称获取属性的索引。 |
| [Remove](./remove/) | 从集合中删除具有指定名称的属性。 |
| [RemoveAt](./removeat/) | 删除指定索引处的属性。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
