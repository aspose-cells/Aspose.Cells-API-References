---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeHtmlSaveOptions. Общие параметры для сохранения html"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

Общие параметры сохранения HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Примечания

Когда указана одна экземпляр [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/), [`SaveFormat`](../saveformat/) будет перезаписан (если он был указан ранее).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Создать параметры сохранения low-code HTML
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Отобразить текущую настройку экспорта линий сетки
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Сохранить с видимыми линиями сетки
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // Изменить параметры HTML, чтобы скрыть линии сетки
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Сохранить без линий сетки
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


