---
title: add_date_filter方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---
##  add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}
添加日期过滤器。



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_index | int |要作为过滤器基础的字段的整数偏移量<br/>（从列表的左边开始；最左边的字段是字段 0）。|
| date_time_grouping_type | [DateTimeGroupingType](/cells/zh/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/zh/python-net/aspose.cells/datetimegroupingtype) |
| year | int |那一年。|
| month | int |这个月。|
| day | int |那天。|
| hour | int |小时。|
| minute | int |分钟。|
| second | int |第二。|
### 评论

如果 DateTimeGroupingType 是 Year，则只有参数年份有效。
如果 DateTiemGroupingType 是 Month，则只有 param year 和 month 有效。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [AutoFilter](/cells/zh/python-net/aspose.cells/autofilter)
* 类 [DateTimeGroupingType](/cells/zh/python-net/aspose.cells/datetimegroupingtype)
