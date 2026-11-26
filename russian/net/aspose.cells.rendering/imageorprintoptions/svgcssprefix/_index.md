---
title: "ImageOrPrintOptions.SvgCssPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает и задаёт префикс имени css в svg. Значение по умолчанию — пустая строка"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Получает и задает префикс имени CSS в SVG, значение по умолчанию — пустая строка.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [`CssPrefix`](../../svgimageoptions/cssprefix/). Это свойство будет удалено через 12 месяцев, начиная с апреля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySvgCssPrefixDemo
    {
        public static void Run()
        {
            string prefix = "custom_prefix_";

            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("SVG CSS Prefix Test");

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            options.OnePagePerSheet = true;
            options.SvgCssPrefix = prefix;

            SheetRender renderer = new SheetRender(workbook.Worksheets[0], options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string svgContent = reader.ReadToEnd();
                    Console.WriteLine("SVG contains CSS prefix: " + svgContent.Contains(prefix + "f"));
                }
            }
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


