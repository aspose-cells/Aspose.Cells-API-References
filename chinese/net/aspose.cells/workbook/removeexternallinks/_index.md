---
title: "Workbook.RemoveExternalLinks"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 方法。删除工作簿中的所有外部链接"
type: docs
url: /zh/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

删除工作簿中的所有外部链接。

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### 备注

注意：此成员现已过时。请改用 ExternalLinkCollection.Clear() 方法。此方法将在自 2021 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些上下文数据
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 调用 RemoveExternalLinks 方法
                workbook.RemoveExternalLinks();

                // 显示方法调用的结果或影响
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // 如果已进行更改，请保存工作簿
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


