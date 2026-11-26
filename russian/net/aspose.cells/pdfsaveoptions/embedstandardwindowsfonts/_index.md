---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. True, чтобы встраивать шрифты TrueType. Влияет только на символы ASCII с кодом 32127. Шрифты для кодов символов больше 127 всегда встраиваются. Шрифты всегда встраиваются для стандартов PDF/A1a и PDF/A1b. По умолчанию — true"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True — встраивать шрифты TrueType. Применяется только к символам ASCII 32‑127. Шрифты для кодов символов больше 127 всегда встраиваются. Шрифты всегда встраиваются для стандарта PDF/A-1a, PDF/A-1b. Значение по умолчанию — true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // Установите параметры сохранения PDF с свойством EmbedStandardWindowsFonts
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Сохранить в поток памяти
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Продемонстрируйте отключение встраивания шрифтов
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


