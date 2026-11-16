---
title: "WorkbookMetadata 类"
linktitle: "WorkbookMetadata"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WorkbookMetadata 类。封装在 Go 中表示 workbookmetadata 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/workbookmetadata/
---

## WorkbookMetadata class

表示元数据。

```go

type WorkbookMetadata struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewWorkbookMetadata_String_MetadataOptions](./newworkbookmetadata_string_metadataoptions/) | 创建元数据对象。 |
| [NewWorkbookMetadata_Stream_MetadataOptions](./newworkbookmetadata_stream_metadataoptions/) | 创建元数据对象。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetOptions](./getoptions/) | 获取元数据的选项。 |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有内置文档属性。 |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有自定义文档属性。 |
| [Save_String](./save_string/) | 将修改后的元数据保存到文件。 |
| [Save_Stream](./save_stream/) | 将修改后的元数据保存到流。 |
