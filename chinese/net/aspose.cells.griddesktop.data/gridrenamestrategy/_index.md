---
title: "枚举 GridRenameStrategy"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy 枚举。列重复名称的策略选项"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

列重复名称的策略选项。

```csharp
public enum GridRenameStrategy
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Exception | `0` | 抛出异常。 |
| Digit | `1` | 使用数字命名。重复的名称将变为 ...1、...2 等。 |
| Letter | `2` | 使用字母命名。重复的名称将变为 ...A、...B 等。 |

### 备注

在处理带有标题的数据时，某些场景要求所有列的标题不重复。例如，在将数据导出到数据表且标题需要作为数据表的列名时，标题的重复值是无效的。对于此类情况，用户可以通过指定此策略来决定如何处理它们。

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


