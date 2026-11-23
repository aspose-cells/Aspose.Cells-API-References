---
title: "枚举 FilterCategory"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.FilterCategory 枚举。表示过滤器的类别"
type: docs
url: /zh/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

表示过滤器的类别。

```csharp
public enum FilterCategory
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无过滤器。 |
| Label | `1` | 标题过滤器。 |
| NumberValue | `2` | 数字值过滤器。 |
| Date | `3` | 日期值过滤器。 |
| Top10 | `4` | Top10 值过滤器。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            CreateSampleData(worksheet);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 配置行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // 配置数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // 向数据透视过滤器添加标签过滤器
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // 演示 FilterCategory 的用法
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // 在数据透视表中显示所有过滤器类别
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // 刷新并计算数据透视表
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存结果
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // 设置示例数据标题
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // 添加示例数据行
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


