---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RevisionLogCollection 方法。突出显示共享工作簿的更改"
type: docs
url: /zh/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

突出显示共享工作簿的更改。

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | HighlightChangesOptions | 设置用于过滤应跟踪的更改的选项。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加一些示例数据和修订
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // 使用选项突出显示更改
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


