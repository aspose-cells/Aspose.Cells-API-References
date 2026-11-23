---
title: "FilterColumn.ColorFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取用于按颜色过滤数据的 ColorFilter"
type: docs
url: /zh/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

获取用于按颜色过滤数据的 [`ColorFilter`](../../colorfilter/)。

```csharp
public ColorFilter ColorFilter { get; }
```

### 备注

首先将 [`FilterType`](../filtertype/) 设置为 ColorFilter，否则将返回 Null。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加带颜色的示例数据
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // 应用自动筛选
                worksheet.AutoFilter.Range = "A1:A4";

                // 获取筛选列
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // 访问 ColorFilter 属性（只读）
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // 显示 ColorFilter 属性
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // 保存工作簿
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


