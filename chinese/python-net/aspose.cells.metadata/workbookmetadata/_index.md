---
title: WorkbookMetadata类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
## WorkbookMetadata类
表示元数据。



WorkbookMetadata 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) |创建元数据对象。|
| [WorkbookMetadata(stream, options)](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) |创建元数据对象。|


### 特性
|属性|描述|
| :- | :- |
| [options](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/options) |获取元数据的选项。|
| [built_in_document_properties](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |返回代表电子表格所有内置文档属性的 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 集合。|
| [custom_document_properties](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) |返回代表电子表格所有自定义文档属性的 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 集合。|


### 方法
|方法|描述|
| :- | :- |
| [save(file_name)](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/save/#str) |将修改后的元数据保存到文件中。|
| [save(stream)](/cells/zh/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) |将修改后的元数据保存到流中。|



### 例子

以下示例创建一个 WorkbookMetadata。

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.metadata](..)
* 类 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty)
