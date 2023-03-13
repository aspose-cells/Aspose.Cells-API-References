---
title: index_of方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.properties/builtindocumentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
按名称获取属性的索引。


### 返回

零基指数。如果找不到则为负值。


```python
def index_of(self, name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| name | str |属性的不区分大小写的名称。|


##  index_of(item, index) {#DocumentProperty-int}
搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。


### 返回

如果找到，从 startIndex 延伸到最后一个元素的数组列表中元素范围内第一次出现值的从零开始的索引；否则，-1。


```python
def index_of(self, item, index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| item | [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) |要在数组列表中定位的对象。该值可以为空。|
| index | int |搜索的从零开始的起始索引。 0（零）在空列表中有效。|


##  index_of(item, index, count) {#DocumentProperty-int-int}
搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。


### 返回

数组列表中元素范围内第一次出现值的从零开始的索引，该范围从 startIndex 开始并包含 count 个元素（如果找到）；否则，-1。


```python
def index_of(self, item, index, count):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| item | [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) |要在数组列表中定位的对象。该值可以为空。|
| index | int |搜索的从零开始的起始索引。 0（零）在空列表中有效。|
| count | int |要搜索的部分中的元素数。|



### 也可以看看
* 模块 [aspose.cells.properties](../../)
* 类 [BuiltInDocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/builtindocumentpropertycollection)
