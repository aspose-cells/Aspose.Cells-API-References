---
title: CustomDocumentPropertyCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
## CustomDocumentPropertyCollection类
自定义文档属性的集合。



**继承：** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/documentpropertycollection)



CustomDocumentPropertyCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [index_of(name)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) |按名称获取属性的索引。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add(name, value)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) |创建一个新的自定义文档属性**属性类型.String**数据类型。|
| [add(name, value)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) |创建一个新的自定义文档属性**属性类型.编号**数据类型。|
| [add(name, value)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) |创建一个新的自定义文档属性**属性类型.日期时间**数据类型。|
| [add(name, value)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) |创建一个新的自定义文档属性**PropertyType.布尔值**数据类型。|
| [add(name, value)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) |创建一个新的自定义文档属性**属性类型.Float**数据类型。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|
| [add_link_to_content(name, source)](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) |创建链接到内容的新自定义文档属性。|
| [update_linked_property_value()](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) |更新链接到内容的自定义文档属性值。|
| [update_linked_range()](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) |将自定义文档属性值更新为链接范围。|



### 评论

每个 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 对象代表容器文档的一个自定义属性。

### 例子

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

### 也可以看看
* 模块 [aspose.cells.properties](..)
* 类 [CustomDocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection)
* 类 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty)
* 类 [DocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/documentpropertycollection)
