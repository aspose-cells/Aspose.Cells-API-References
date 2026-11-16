---
title: "ErrorCheckType 枚举"
linktitle: "ErrorCheckType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ErrorCheckType 枚举。封装在 Go 中表示 errorchecktype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

表示所有错误检查类型。

```go

type ErrorCheckType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [EvaluationError](./evaluationerror/) | 当单元格包含导致错误的公式时忽略错误。 |
| [EmptyCellRef](./emptycellref/) | 当公式引用空单元格时忽略错误。 |
| [NumberStoredAsText](./numberstoredastext/) | 当数字被格式化为文本或前面带有撇号时忽略错误 |
| [InconsistRange](./inconsistrange/) | 当公式在区域中省略某些单元格时忽略错误。 |
| [InconsistFormula](./inconsistformula/) | 当工作表区域中的公式与同一区域的其他公式不同时忽略错误。 |
| [TwoDigitTextYear](./twodigittextyear/) | 当公式包含以两位数字表示年份的文本格式单元格时忽略错误。 |
| [UnlockedFormula](./unlockedformula/) | 当未锁定的单元格包含公式时忽略错误。 |
| [TableDataValidation](./tabledatavalidation/) | 当表格中单元格的值不符合指定的数据验证规则时忽略错误。 |
| [CalculatedColumn](./calculatedcolumn/) | 当单元格包含与计算列公式不同的值时，忽略错误。 |
