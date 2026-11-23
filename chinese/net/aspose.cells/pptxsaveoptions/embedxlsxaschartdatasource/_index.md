---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PptxSaveOptions 属性。指示是否将 xlsx 文件嵌入为图表的数据源"
type: docs
url: /zh/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

指示是否将 xlsx 文件嵌入为图表的数据源。

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### 备注

默认值为 true。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建包含图表数据的示例工作表
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // 添加图表以演示该属性的效果
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // 创建 PptxSaveOptions 实例
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // 显示 EmbedXlsxAsChartDataSource 的默认值
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // 将属性设置为 true 以演示其用法
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // 在启用该选项的情况下将工作簿保存为 PPTX
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


