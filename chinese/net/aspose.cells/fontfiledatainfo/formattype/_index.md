---
title: "FontFileDataInfo.FormatType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FontFileDataInfo 属性。获取字体文件的字体格式类型"
type: docs
url: /zh/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

获取字体文件的字体格式类型。

```csharp
public FontFileFormatType FormatType { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些文本以演示字体使用
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // 加载示例字体文件（请替换为实际的字体文件路径）
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // 注册字体文件夹
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // 在真实场景中，FontFileDataInfo 将从库中获取
                    // 为了演示，我们将模拟获取字体信息
                    // 注意：实际 API 可能通过 FontConfigs 或类似方式提供此功能
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // 显示 FormatType 属性值
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // 将枚举值显示为字符串
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // 将字体应用于单元格（概念性 - 实际实现可能有所不同）
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // 保存工作簿
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // 帮助方法，用于模拟获取 FontFileDataInfo
        // 在实际使用中，这将由 Aspose.Cells API 提供
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // 创建一个模拟的 FontFileDataInfo（实际上，这将来自 API）
                // 由于我们无法直接实例化它，我们将模拟其行为
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // 在真实实现中，这将由 API 返回
                // 对于此演示，我们只能返回 null，因为我们无法创建该对象
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### 另请参见

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


