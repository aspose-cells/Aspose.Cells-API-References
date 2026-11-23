---
title: "TextOptions.LanguageCode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextOptions 属性。获取并设置用户界面语言"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

获取并设置用户界面语言。

```csharp
public CountryCode LanguageCode { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加形状并设置其文本
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // 为形状的文本选项设置语言代码
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // 验证并输出语言代码
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // 保存工作簿
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


