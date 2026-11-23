---
title: "PivotFilter.GetNumberValues"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilter 方法。获取数字过滤器的值"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

获取数字过滤器的值。

```csharp
public double[] GetNumberValues()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetNumberValuesDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 5;
            sheet.Cells["B3"].Value = 3;
            sheet.Cells["B4"].Value = 2;

            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 应用值过滤器
            pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
            
            // 获取并显示过滤器值
            PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
            double[] numberValues = filter.GetNumberValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
        }
    }
}
```

### 另请参见

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


