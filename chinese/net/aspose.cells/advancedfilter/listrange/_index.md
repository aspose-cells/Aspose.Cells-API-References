---
title: "AdvancedFilter.ListRange"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AdvancedFilter 属性。获取此高级筛选器的列表范围"
type: docs
url: /zh/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

获取此高级筛选的列表范围。

```csharp
public string ListRange { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 填充示例数据
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // 设置高级筛选
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange 为只读，并在创建筛选器时自动设置
            // 我们只能读取它，不能直接设置
            
            // 显示列表范围（将显示自动确定的范围）
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // 保存工作簿
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


