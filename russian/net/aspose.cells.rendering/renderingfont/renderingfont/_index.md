---
title: "RenderingFont.RenderingFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор RenderingFont. Инициализирует новый экземпляр RenderingFont"
type: docs
url: /ru/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Инициализирует новый экземпляр [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | String | название шрифта |
| fontSize | Single | размер шрифта в пунктах |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте шрифт, используя конструктор #ctor(string, single)
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Создайте стиль и задайте шрифт
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Примените стиль к ячейке
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


