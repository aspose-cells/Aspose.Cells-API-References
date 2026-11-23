---
title: "PivotField.GetFilters"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。获取此透视字段已应用的所有透视筛选器"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

获取此透视字段已应用的所有透视筛选器。

```csharp
public PivotFilter[] GetFilters()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFiltersDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["B1"].Value = "Sales";
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
                worksheet.Cells[$"B{i}"].Value = i * 100;
            }

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // 添加行字段和数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 应用日期筛选
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = DateTime.Now;
            DateTime endDate = DateTime.Now.AddDays(5);
            dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
            
            // 获取并显示筛选器
            PivotFilter[] filters = dateField.GetFilters();
            Console.WriteLine($"Number of filters applied: {filters.Length}");
            if (filters.Length > 0)
            {
                Console.WriteLine($"Filter type: {filters[0].FilterType}");
                Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
                Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
            }
            
            // 保存工作簿
            workbook.Save("PivotFieldGetFiltersDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


