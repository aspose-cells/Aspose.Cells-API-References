---
title: "类 AdvancedFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.AdvancedFilter 类。表示高级筛选的设置"
type: docs
url: /zh/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

表示高级筛选的设置。

```csharp
public class AdvancedFilter
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | 获取将此高级筛选结果复制到的范围。 |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | 获取此高级筛选的条件范围。 |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | 获取此高级筛选的列表范围。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 为列表范围填充示例数据
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // 填充条件范围
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // 从工作表获取 AdvancedFilter 实例
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // 显示只读属性
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // 保存工作簿
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


