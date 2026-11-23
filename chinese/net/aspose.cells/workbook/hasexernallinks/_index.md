---
title: "Workbook.HasExernalLinks"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 方法。指示此工作簿是否包含指向其他数据源的外部链接"
type: docs
url: /zh/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

指示此工作簿是否包含指向其他数据源的外部链接。

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### 返回值

此工作簿是否包含指向其他数据源的外部链接。

### 备注

注意：此成员现已过时。请改用 ExternalLinkCollection.Count 来检查此工作簿中是否存在外部链接。此方法将在自 2021 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // 创建带有外部链接的工作簿
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // 添加外部链接
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // 检查工作簿是否有外部链接
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### 另请参见

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


