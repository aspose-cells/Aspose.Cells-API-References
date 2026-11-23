---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。指示是否将 xlsx 文件嵌入为图表的数据源"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

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
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表并添加示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // 初始化 DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // 显示 EmbedXlsxAsChartDataSource 属性的默认值
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // 将 EmbedXlsxAsChartDataSource 设置为 true 以演示其用法
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // 使用配置的选项将工作簿保存为 DOCX
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


