---
title: "ExternalLinkCollection 类"
linktitle: "ExternalLinkCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ExternalLinkCollection 类。封装在 Go 中表示 externallinkcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/externallinkcollection/
---

## ExternalLinkCollection class

表示工作簿中外部链接的集合。

```go

type ExternalLinkCollection struct  {
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
| [GetCount](./getcount/) | 获取集合实际包含的元素数量。 |
| [Add_String_stringArray](./add_string_stringarray/) | 添加外部链接。 |
| [Add_DirectoryType_String_stringArray](./add_directorytype_string_stringarray/) | 添加外部链接。 |
| [Get](./get/) | 获取指定索引处的 ExternalLink 元素。 |
| [Clear](./clear/) | 移除所有外部链接。 |
| [Clear_Bool](./clear_bool/) | 移除所有外部链接。 |
| [RemoveAt_Int](./removeat_int/) | 从工作簿中移除指定的外部链接。 |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | 从工作簿中移除指定的外部链接。 |
| [GetEnumerator](./getenumerator/) | 获取一个遍历此集合的枚举器。 |
