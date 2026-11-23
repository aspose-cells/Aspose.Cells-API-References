---
title: "FindOptions.SearchNext"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FindOptions 属性。搜索顺序。True 表示搜索下一个。False 表示搜索上一个"
type: docs
url: /zh/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

搜索顺序。True：搜索下一个。False：搜索上一个。

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### 备注

注意：此成员已过时。请改用 FindOptions.SearchBackward 属性。该属性将在自 2018 年 11 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 填充一些示例数据
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // 创建查找选项
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // 演示 SearchNext 属性（已过时，但为演示而展示）
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // 向前搜索（默认行为）
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // 向后搜索
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // 保存工作簿
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


