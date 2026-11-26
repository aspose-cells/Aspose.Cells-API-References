---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает тип встраиваемого шрифтового файла в html. Значение по умолчанию — None, что указывает, что шрифт не будет встраиваться в html."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Получает или задаёт тип встраивания файлов шрифтов в HTML‑файл. Значение по умолчанию — None, что означает, что шрифты не будут встраиваться в HTML.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Создать параметры сохранения HTML
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Отобразите значение EmbeddedFontType по умолчанию
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Установите EmbeddedFontType в Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Сохраните рабочую книгу с встраиванием шрифта WOFF
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Сбросить в None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Сохраните рабочую книгу без встраивания шрифта
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


