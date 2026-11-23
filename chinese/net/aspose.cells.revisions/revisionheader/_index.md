---
title: "类 RevisionHeader"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Revisions.RevisionHeader 类。表示此工作簿中已发生的特定更改列表"
type: docs
url: /zh/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

表示此工作簿中已发生的特定更改列表。

```csharp
public class RevisionHeader
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RevisionHeader](revisionheader/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | 获取并设置此修订集保存时的日期和时间。 |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | 获取并设置进行修订的用户名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建 RevisionHeader 类的实例
                RevisionHeader revisionHeader = new RevisionHeader();

                // 设置必要属性
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // 演示基本功能
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // 保存工作簿
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


