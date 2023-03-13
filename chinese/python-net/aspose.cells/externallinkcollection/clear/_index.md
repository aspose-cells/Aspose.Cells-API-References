---
title: clear方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
删除所有外部链接。



```python
def clear(self):
    ...
```


### 评论

删除外部链接时，所有引用它们的公式也将被删除，因为
引用变得无效。

##  clear(update_references_as_local) {#bool}
删除所有外部链接。



```python
def clear(self, update_references_as_local):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| update_references_as_local | bool |是否将外部链接的所有引用更新为当前工作簿本身的引用。|
### 评论

如果需要更新引用，则公式中对外部链接的引用将更改为当前工作簿。
比如一个单元格的原始公式是“='externalsource.xlam'!customfunction()”，
删除外部链接后，公式将变为“=customfunction()”。
如果不需要更新引用，则所有引用外部链接的公式
也将被删除，因为这些引用变得无效。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [ExternalLinkCollection](/cells/zh/python-net/aspose.cells/externallinkcollection)
