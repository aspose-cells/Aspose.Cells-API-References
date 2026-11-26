---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, следует ли разбирать HTML‑теги, такие как div/div, в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Указывает, следует ли разбирать HTML‑теги (например, `<div></div>`) в ячейке как значение ячейки или сохранять их как есть. Значение по умолчанию — true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с примерными данными, содержащими HTML‑теги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить значение ячейки с HTML‑тегами
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Создать параметры сохранения HTML и включить разбор HTML‑тегов
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Сохранить рабочую книгу с разобранными HTML‑тегами
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


