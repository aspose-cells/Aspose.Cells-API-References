---
title: "AdvancedFilter.CriteriaRange"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AdvancedFilter 属性。获取此高级筛选器的条件范围"
type: docs
url: /zh/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

获取此高级筛选的条件范围。

```csharp
public string CriteriaRange { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 为列表范围填充示例数据
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // 填充示例条件（筛选器在应用时将使用此条件）
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // 获取工作表的 AdvancedFilter 对象
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // ListRange、CriteriaRange 和 CopyToRange 属性是只读的。
                // 显示自动确定的范围。
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // 保存工作簿（可选，仅用于显示文件可以被创建）
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


