---
title: "类 FontFileDataInfo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.FontFileDataInfo 类。表示字体文件数据的信息"
type: docs
url: /zh/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

表示字体文件数据的信息。

```csharp
public class FontFileDataInfo
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | 获取字体文件的二进制数据。 |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | 获取字体文件的字体格式类型。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 示例：加载字体文件数据
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // 注意：FontFileDataInfo 不能直接实例化，因为它没有公共构造函数
            // 并且其属性是只读的。在实际场景中，您将获取一个实例
            // 来自另一个 API 方法（如 FontConfigs.GetFontFileDataInfo()）
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // 演示如果我们拥有实例时属性的使用方式
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // 演示与 Workbook 的集成
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // 保存工作簿
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


