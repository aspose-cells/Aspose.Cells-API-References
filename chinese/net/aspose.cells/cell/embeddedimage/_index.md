---
title: "Cell.EmbeddedImage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 属性。获取并设置单元格中的嵌入图像"
type: docs
url: /zh/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

获取并设置单元格中的嵌入图像。

```csharp
public byte[] EmbeddedImage { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // 创建新工作簿并获取第一个工作表
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 选择一个单元格来存储嵌入图像
                Cell cell = worksheet.Cells["B2"];

                // 一个 1x1 像素的透明 PNG（Base64 编码）
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // 将 Base64 字符串转换为字节数组
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // 将嵌入的图像设置到单元格中
                cell.EmbeddedImage = imageBytes;

                // 从单元格中检索嵌入的图像
                byte[] retrievedBytes = cell.EmbeddedImage;

                // 将检索到的图像写入文件，以验证其已正确存储
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // 保存工作簿（嵌入的图像存储在 .xlsx 文件中）
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


