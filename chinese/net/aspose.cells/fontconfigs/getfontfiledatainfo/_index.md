---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FontConfigs 方法。获取字体文件数据的信息"
type: docs
url: /zh/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

获取字体文件数据的信息。

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontName | String | 字体名称 |
| isBold | 布尔 | 字体样式是否为粗体 |
| isItalic | 布尔 | 字体样式是否为斜体 |
| isExactStyle | 布尔 | 是否精确匹配给定的粗体/斜体样式 |

### 返回值

字体文件数据的信息。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // 使用特定参数调用 GetFontFileDataInfo（已更改为静态调用）
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // 显示关于字体文件数据的信息
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // 演示在工作簿上的效果
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // 使用我们检查的字体设置样式
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // 将样式应用于单元格
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // 保存工作簿
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


