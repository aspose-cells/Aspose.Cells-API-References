---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, добавлять ли общий шрифт в CSS fontfamily. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Указывает, следует ли добавить общий шрифт в CSS‑font-family. Значение по умолчанию: true

```csharp
public bool AddGenericFont { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddGenericFontDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пример текста с определённым шрифтом
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // Сохранить с включённым AddGenericFont (по умолчанию)
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // Сохранить с отключённым AddGenericFont
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Проверьте результаты
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


