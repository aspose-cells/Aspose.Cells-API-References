---
title: remove_at方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
从工作簿中删除指定的外部链接。



```python
def remove_at(self, index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| index | int |要删除的外部链接的索引。|
### 评论

删除外部链接时，所有引用它的公式也将被删除，因为
引用变得无效。

##  remove_at(index, update_references_as_local) {#int-bool}
从工作簿中删除指定的外部链接。



```python
def remove_at(self, index, update_references_as_local):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| index | int |要删除的外部链接的索引。|
| update_references_as_local | bool |是否将给定外部链接的所有引用更新为当前工作簿本身的引用。|
### 评论

如果需要更新引用，则公式中对外部链接的引用将更改为当前工作簿。
例如，要删除的外部链接是“externalsource.xlam”，它定义了一个自定义函数“customfunction()”，
一个单元格的原始公式是“='externalsource.xlam'!customfunction()”，
删除公式后将变为“=customfunction()”。
如果不需要更新引用，则所有引用此外部链接的公式
也将被删除，因为这些引用变得无效。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [ExternalLinkCollection](/cells/zh/python-net/aspose.cells/externallinkcollection)
