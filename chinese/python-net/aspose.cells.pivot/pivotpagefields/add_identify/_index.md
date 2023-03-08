---
title: add_identify方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
设置每个页面字段中用于标识数据范围的项目标签。
pageItemIndex.Length 必须等于PageFieldCount，所以请先添加页面字段。



```python
def add_identify(self, range_index, page_item_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| range_index | int |合并数据范围索引。|
| page_item_index | list |每个页面字段中的页面项目索引。<br/>pageItemIndex[2] = 1 表示第三个字段中的第二个项目用于标识此范围。<br/> pageItemIndex[1] = -1 表示第二个字段中没有项目可用于标识此范围<br/>MS 将在第二个字段中自动创建“空白”项以标识此范围。|



### 也可以看看
* 模块 [aspose.cells.pivot](../../)
* 类 [PivotPageFields](/cells/zh/python-net/aspose.cells.pivot/pivotpagefields)
