---
title: "PivotTableFormat.GetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableFormat 方法。获取已格式化的样式"
type: docs
url: /zh/net/aspose.cells.pivot/pivottableformat/getstyle/
---
## PivotTableFormat.GetStyle method

获取已格式化的样式。

```csharp
public Style GetStyle()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableFormatMethodGetStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 获取数据透视表格式
            PivotTableFormatCollection formats = pivotTable.PivotFormats;
            PivotTableFormat format = formats[0];

            try
            {
                // 调用 GetStyle 方法
                Style style = format.GetStyle();

                // 显示样式属性
                Console.WriteLine("Style properties:");
                Console.WriteLine($"Font Name: {style.Font.Name}");
                Console.WriteLine($"Font Size: {style.Font.Size}");
                Console.WriteLine($"Background Color: {style.BackgroundColor}");

                // 修改样式
                style.Font.Name = "Arial";
                style.Font.Size = 12;
                style.BackgroundColor = System.Drawing.Color.LightBlue;

                // 将修改后的样式应用回格式
                format.SetStyle(style);

                Console.WriteLine("GetStyle method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


