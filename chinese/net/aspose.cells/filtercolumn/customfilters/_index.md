---
title: "FilterColumn.CustomFilters"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取 CustomFilterCollection 以通过自定义条件过滤数据"
type: docs
url: /zh/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

获取 [`CustomFilterCollection`](../../customfiltercollection/) 以通过自定义条件过滤数据。

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### 备注

注意：此属性的 setter 已过时。请改为使用属性 [`FilterType`](../filtertype/) 并将其设置为 CustomFilters。此属性将在自 2026 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加示例数据
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // 应用自动筛选
                worksheet.AutoFilter.Range = "A1:A6";

                // 获取筛选列
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // 使用 AutoFilter.Custom 方法创建并设置自定义筛选器
                // 第一个筛选器：以 "A" 开头
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // 第二个筛选器：以 "y" 结尾（AND 关系）
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // 从筛选列获取自定义筛选器
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // 显示自定义筛选器信息
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // 注意：CustomFilterCollection 不直接公开单个筛选器
                // 通过索引器，因此我们只能显示集合属性
                Console.WriteLine("Custom filters have been applied to the column.");

                // 保存工作簿
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


