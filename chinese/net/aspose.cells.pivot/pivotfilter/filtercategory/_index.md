---
title: "PivotFilter.FilterCategory"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilter 属性。获取此过滤器的类别"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfilter/filtercategory/
---
## PivotFilter.FilterCategory property

获取此过滤器的类别。

```csharp
public FilterCategory FilterCategory { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyFilterCategoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建示例透视表数据
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                worksheet.Cells["B1"].Value = "Value";
                worksheet.Cells["B2"].Value = 100;
                worksheet.Cells["B3"].Value = 200;
                worksheet.Cells["B4"].Value = 300;

                // 创建数据透视表
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // 使用正确的 API 方法添加行字段
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                
                // 使用正确的 API 方法添加数据字段
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;
                dataField.DisplayName = "Total";

                // 向 Category 字段添加标题过滤器
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // 显示 FilterCategory 属性值
                Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);

                workbook.Save("FilterCategoryDemo.xlsx");
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

* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


