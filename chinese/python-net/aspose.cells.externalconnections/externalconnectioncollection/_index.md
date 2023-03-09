---
title: ExternalConnectionCollection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
## ExternalConnectionCollection类
指定 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection) 集合



ExternalConnectionCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [copy_to(array)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [get_external_connection_by_id(conn_id)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) |获取具有指定 ID 的 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection) 元素。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

wb = Workbook("connection.xlsx")
dataConns = wb.data_connections
dataConn = None
for i in range(len(dataConns)):
    dataConn = dataConns[i]
    # get external connection id
    print(dataConn.connection_id)

```

### 也可以看看
* 模块 [aspose.cells.externalconnections](..)
* 类 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)
