---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SvgImageOptions. Получает или задает тип шрифта, который встраивается в Svg"
type: docs
url: /ru/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

Получает или задает тип шрифта, встроенного в SVG.

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### Примечания

Значение по умолчанию — None, что указывает на то, что шрифт не будет встраиваться в Svg.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте данные с пользовательским форматированием, чтобы продемонстрировать встраивание шрифта
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Создать параметры рендеринга SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Отобразить начальный тип встроенного шрифта
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // Отрисовать лист в SVG без встраивания шрифта
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // Изменить тип встроенного шрифта на WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // Отрисовать лист в SVG с встраиванием шрифта WOFF
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### См. также

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


