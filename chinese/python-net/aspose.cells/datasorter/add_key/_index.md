---
title: add_key方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/datasorter/add_key/
is_root: false
---
##  add_key(key, order) {#int-SortOrder}
添加排序列索引和排序顺序。



```python
def add_key(self, key, order):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| key | int |排序后的列索引（绝对位置，A列为0，B列为1，...）|
| order | [SortOrder](/cells/zh/python-net/aspose.cells/sortorder) |排序顺序|


##  add_key(key, order, custom_list) {#int-SortOrder-str}
使用自定义排序列表添加排序列索引和排序顺序。



```python
def add_key(self, key, order, custom_list):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| key | int |排序后的列索引（绝对位置，A列为0，B列为1，...）|
| order | [SortOrder](/cells/zh/python-net/aspose.cells/sortorder) |排序顺序。|
| custom_list | str |自定义排序列表。|


##  add_key(key, order, custom_list) {#int-SortOrder-list}
使用自定义排序列表添加排序列索引和排序顺序。



```python
def add_key(self, key, order, custom_list):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| key | int |排序后的列索引（绝对位置，A列为0，B列为1，...）|
| order | [SortOrder](/cells/zh/python-net/aspose.cells/sortorder) |排序顺序。|
| custom_list | list |自定义排序列表。|


##  add_key(key, type, order, custom_list) {#int-SortOnType-SortOrder-any}
使用自定义排序列表添加排序列索引和排序顺序。



```python
def add_key(self, key, type, order, custom_list):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| key | int |排序后的列索引（绝对位置，A列为0，B列为1，...）|
| type | [SortOnType](/cells/zh/python-net/aspose.cells/sortontype) |已排序的值类型。|
| order | [SortOrder](/cells/zh/python-net/aspose.cells/sortorder) |排序顺序。|
| custom_list | any |自定义排序列表。|
### 评论

如果类型是 SortOnType.CellColor 或 SortOnType.FontColor，则 customList 是 Color。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [DataSorter](/cells/zh/python-net/aspose.cells/datasorter)
