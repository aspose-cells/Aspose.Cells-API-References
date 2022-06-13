---
title: RemoveDateFilter
second_title: Aspose.Cells for .NET API 参考
description: 删除日期过滤器
type: docs
weight: 180
url: /zh/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

删除日期过滤器。

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | Int32 | 要作为过滤器基础的字段的整数偏移量 （从左侧列表的；最左边的字段是字段 0)。 |
| dateTimeGroupingType | DateTimeGroupingType | [`DateTimeGroupingType`](../../datetimegroupingtype) |
| year | Int32 | 年份。 |
| month | Int32 | 月份。 |
| day | Int32 | 当天。 |
| hour | Int32 | 小时。 |
| minute | Int32 | 分钟。 |
| second | Int32 | 秒。 |

### 评论

如果 DateTimeGroupingType 为 Year，则只有参数年份有效。 如果 DateTiemGroupingType 为 Month，则只有参数年月效果。

### 也可以看看

* enum [DateTimeGroupingType](../../datetimegroupingtype)
* class [AutoFilter](../../autofilter)
* 命名空间 [Aspose.Cells](../../autofilter)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->