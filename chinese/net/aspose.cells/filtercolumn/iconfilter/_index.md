---
title: "FilterColumn.IconFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FilterColumn 属性。获取 IconFilter 以通过图标过滤数据"
type: docs
url: /zh/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

获取 `IconFilter` 以通过图标过滤数据。

```csharp
public IconFilter IconFilter { get; }
```

### 备注

在使用此属性之前，请确保 [`FilterType`](../filtertype/) 为 IconFilter，否则将返回 null。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加使用图标的条件格式示例数据
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // 对范围应用自动筛选
                worksheet.AutoFilter.Range = "A1:A5";

                // 获取筛选列
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // 访问 IconFilter 属性（只读）
                IconFilter iconFilter = filterColumn.IconFilter;

                // 如果存在，则显示 IconFilter 属性
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // 保存工作簿
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


