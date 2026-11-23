---
title: "Chart.ChangeTemplate"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Chart 方法。使用预设模板更改图表类型"
type: docs
url: /zh/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

使用预设模板更改图表类型。

```csharp
public void ChangeTemplate(byte[] data)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数据 | Byte[] | 图表模板文件（.crtx）的数据。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // 设置图表数据范围
            chart.SetChartDataRange("A1:B4", false);

            // 从另一个图表文件获取模板数据
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // 使用字节数组参数调用 ChangeTemplate 方法
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // 通过保存工作簿来显示效果
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


