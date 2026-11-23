---
title: "类 HighlightChangesOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Revisions.HighlightChangesOptions 类。表示对共享 Excel 文件的修订或更改进行高亮显示的选项"
type: docs
url: /zh/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

表示对共享 Excel 文件的修订或更改进行高亮显示的选项。

```csharp
public class HighlightChangesOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | 表示对共享 Excel 文件的修订或更改进行高亮显示的选项。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // 实例化 Workbook 对象
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // 获取修订日志
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // 设置保留历史的天数
            revisionLogs.DaysPreservingHistory = 30;

            // 创建 HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // 突出显示更改
            revisionLogs.HighlightChanges(options);

            // 保存带有突出显示更改的工作簿
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


