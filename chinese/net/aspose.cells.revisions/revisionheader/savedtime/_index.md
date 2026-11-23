---
title: "RevisionHeader.SavedTime"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RevisionHeader 属性。获取和设置此修订集保存时的日期和时间"
type: docs
url: /zh/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

获取并设置此修订集保存时的日期和时间。

```csharp
public DateTime SavedTime { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建 RevisionHeader 实例
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // 设置 SavedTime 属性
                revisionHeader.SavedTime = DateTime.Now;
                
                // 获取并显示 SavedTime 值
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // 修改 SavedTime 属性
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // 保存工作簿以演示属性的使用
                workbook.Save("SavedTimeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


