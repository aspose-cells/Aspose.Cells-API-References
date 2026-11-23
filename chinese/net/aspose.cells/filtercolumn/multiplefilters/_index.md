---
title: "FilterColumn.MultipleFilters"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取用于按标签或日期时间过滤数据的 MultipleFilterCollection"
type: docs
url: /zh/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

获取用于按标签或日期时间过滤数据的 [`MultipleFilterCollection`](../../multiplefiltercollection/)。

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### 备注

注意：此成员现已过时。请改用 FilterColumn.FilterValues 属性。此属性将在自 2026 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加示例数据
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // 对范围应用 AutoFilter
                worksheet.AutoFilter.Range = "A1:A5";

                // 获取第一个过滤列
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // 创建并设置 MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // 将 MultipleFilters 分配给过滤列
                filterColumn.MultipleFilters = multipleFilters;

                // 显示 MultipleFilters 属性
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // 保存工作簿
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


