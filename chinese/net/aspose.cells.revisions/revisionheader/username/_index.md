---
title: "RevisionHeader.UserName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RevisionHeader 属性。获取和设置进行修订的用户名称"
type: docs
url: /zh/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

获取并设置进行修订的用户名称。

```csharp
public string UserName { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            try
            {
                // 创建 RevisionHeader 实例
                RevisionHeader revisionHeader = new RevisionHeader();

                // 设置 UserName 属性
                revisionHeader.UserName = "JohnDoe";

                // 显示 UserName 属性的当前值
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // 修改 UserName 属性
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // 保存工作簿以演示属性的使用
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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


