---
title: "FontFileDataInfo.Data"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FontFileDataInfo 属性。获取字体文件的二进制数据"
type: docs
url: /zh/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

获取字体文件的二进制数据。

```csharp
public byte[] Data { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 加载字体文件（请替换为实际的字体文件路径）
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // 创建一个 FontConfigs 实例并添加字体
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // 在实际使用中，FontFileDataInfo 将从库中获取
            // 出于演示目的，我们只展示如果你拥有它时的使用方式
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // 显示字体数据的信息（如果可用）
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // 在实际使用中，将使用 Data 属性来访问字体二进制数据
            // 例如，你可以将其保存到文件：
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // 保存工作簿（如果在单元格中使用，字体会影响渲染）
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


