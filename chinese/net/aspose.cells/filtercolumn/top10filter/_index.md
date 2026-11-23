---
title: "FilterColumn.Top10Filter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取用于按数据排名过滤的 Top10Filter"
type: docs
url: /zh/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

获取用于按数据排名过滤的 `Top10Filter`。

```csharp
public Top10Filter Top10Filter { get; }
```

### 备注

在使用此属性之前，请确保 [`FilterType`](../filtertype/) 为 Top10，否则将返回 null。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // 创建新工作簿并获取第一个工作表
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // 填充一些示例数据
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // 对数据范围应用自动筛选
                sheet.AutoFilter.Range = "A1:A5";

                // 获取第一个筛选列（列索引 0）
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // 显示当前的 Filter 对象（可能为 null）
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // 检查应用的筛选是否为 Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // 保存工作簿（可选）
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


