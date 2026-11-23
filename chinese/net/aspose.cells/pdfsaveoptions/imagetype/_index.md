---
title: "PdfSaveOptions.ImageType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PdfSaveOptions 属性。表示在转换图表和形状时的图像类型"
type: docs
url: /zh/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

表示在转换图表和形状时的图像类型。

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### 备注

注意：此成员已过时。相反，图表和形状始终渲染为矢量元素（例如点、线），以提升渲染质量。此属性将在自2022年6月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建一个包含一些数据的示例工作表
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // 创建 PDF 保存选项
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // 显示默认的 ImageType 值
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // 设置不同的 ImageType 值
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // 使用指定的 ImageType 将工作簿保存为 PDF
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


