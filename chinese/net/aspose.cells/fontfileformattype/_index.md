---
title: "枚举 FontFileFormatType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.FontFileFormatType 枚举。表示字体格式类型"
type: docs
url: /zh/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

表示字体格式类型。

```csharp
public enum FontFileFormatType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Unknown | `0` | 未知的字体格式类型。 |
| Ttf | `1` | TTF 字体格式类型。 |
| Otf | `2` | OTF 字体格式类型。 |
| Ttc | `3` | TTC 字体格式类型。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 访问单元格并设置其样式
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // 演示 FontFileFormatType 的用法
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // 应用字体设置
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // 检查字体格式兼容性
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // 保存工作簿
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


