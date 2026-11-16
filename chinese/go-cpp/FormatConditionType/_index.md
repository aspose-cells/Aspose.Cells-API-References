---
title: "FormatConditionType 枚举"
linktitle: "FormatConditionType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FormatConditionType 枚举。封装在 Go 中表示 formatconditiontype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

条件格式规则类型。

```go

type FormatConditionType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [CellValue](./cellvalue/) | 此条件格式规则使用运算符比较单元格值与公式计算结果。 |
| [Expression](./expression/) | 此条件格式规则包含一个待评估的公式。当公式结果为真时，单元格将被突出显示。 |
| [Top10](./top10/) | 此条件格式规则突出显示其值位于前 N 或后 N 区间的单元格，如指定的那样。 |
| [UniqueValues](./uniquevalues/) | 此条件格式规则突出显示范围内的唯一值。 |
| [DuplicateValues](./duplicatevalues/) | 此条件格式规则突出显示重复的值。 |
| [ContainsText](./containstext/) | 此条件格式规则突出显示包含给定文本的单元格。相当于使用 SEARCH() 工作表函数来判断单元格是否包含该文本。 |
| [NotContainsText](./notcontainstext/) | 此条件格式规则突出显示不包含给定文本的单元格。相当于使用 SEARCH() 工作表函数来判断单元格是否包含该文本。 |
| [BeginsWith](./beginswith/) | 此条件格式规则突出显示范围内以给定文本开头的单元格。相当于使用 LEFT() 工作表函数并比较值。 |
| [EndsWith](./endswith/) | 此条件格式规则突出显示以给定文本结尾的单元格。相当于使用 RIGHT() 工作表函数并比较值。 |
| [ContainsBlanks](./containsblanks/) | 此条件格式规则突出显示完全为空的单元格。相当于使用 LEN(TRIM())。这意味着如果单元格仅包含 TRIM() 会删除的字符，则视为为空。空单元格也视为为空。 |
| [NotContainsBlanks](./notcontainsblanks/) | 此条件格式规则突出显示非空的单元格。相当于使用 LEN(TRIM())。这意味着如果单元格仅包含 TRIM() 会删除的字符，则视为为空。空单元格也视为为空。 |
| [ContainsErrors](./containserrors/) | 此条件格式规则突出显示公式错误的单元格。相当于使用 ISERROR() 工作表函数来判断是否存在公式错误。 |
| [NotContainsErrors](./notcontainserrors/) | 此条件格式规则突出显示没有公式错误的单元格。相当于使用 ISERROR() 工作表函数来判断是否存在公式错误。 |
| [TimePeriod](./timeperiod/) | 此条件格式规则突出显示在指定时间段内包含日期的单元格。会评估单元格的底层值，因此单元格不需要格式化为日期即可进行评估。例如，单元格值为 38913 时，如果规则要求的值为 2006/7/14，则会应用此条件格式。 |
| [AboveAverage](./aboveaverage/) | 此条件格式规则突出显示范围内所有值的平均值以上或以下的单元格。 |
| [ColorScale](./colorscale/) | 此条件格式规则在单元格上创建渐变颜色刻度。 |
| [DataBar](./databar/) | 此条件格式规则在单元格范围内显示渐变数据条。 |
| [IconSet](./iconset/) | 此条件格式规则根据单元格的值向其应用图标。 |
