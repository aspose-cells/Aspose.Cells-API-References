---
title: "FilterColumn.DynamicFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取用于动态条件过滤的 DynamicFilter"
type: docs
url: /zh/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

获取用于动态条件过滤的 `DynamicFilter`。

```csharp
public DynamicFilter DynamicFilter { get; }
```

### 备注

在使用此属性之前，请确保 [`FilterType`](../filtertype/) 为 DynamicFilter，否则将返回 null。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加示例数据
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // 应用自动筛选
                worksheet.AutoFilter.Range = "A1:A4";

                // 获取筛选列
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // 访问 DynamicFilter 属性（只读）
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // 显示 DynamicFilter 属性
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // 保存工作簿
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


