---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置网格线颜色"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

获取或设置网格线颜色。

```csharp
public Color GridlineColor { get; set; }
```

### 备注

它将忽略源文件中的网格线颜色设置。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // 创建 PDF 保存选项
                PdfSaveOptions options = new PdfSaveOptions();

                // 显示默认的 GridlineColor 值
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // 设置新的网格线颜色
                options.GridlineColor = Color.Red;

                // 显示更新后的 GridlineColor 值
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // 使用网格线颜色设置保存工作簿
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


