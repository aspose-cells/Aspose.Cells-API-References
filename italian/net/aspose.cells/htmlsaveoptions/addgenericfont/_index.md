---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se aggiungere un carattere generico alla famiglia di font CSS. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Indica se aggiungere un font generico al CSS font-family. Il valore predefinito è true

```csharp
public bool AddGenericFont { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il testo di esempio con un carattere specifico
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // Salva con AddGenericFont abilitato (predefinito)
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // Salva con AddGenericFont disabilitato
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Verifica i risultati
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


