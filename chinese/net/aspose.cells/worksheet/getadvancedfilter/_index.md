---
title: "Worksheet.GetAdvancedFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Worksheet 方法。获取高级筛选的设置"
type: docs
url: /zh/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

获取高级筛选的设置。

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 设置过滤的数据
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // 设置条件范围
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // 应用高级筛选
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // 获取高级筛选
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // 输出筛选范围
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### 另请参见

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


