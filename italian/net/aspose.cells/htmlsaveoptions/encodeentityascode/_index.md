---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se le entità dei caratteri HTML vengono sostituite con il codice decimale. ad es. nbsp è sostituito con 160. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Indica se le entità dei caratteri html vengono sostituite con il codice decimale. (ad esempio, "&amp;nbsp;" è sostituito con "&amp;#160;"). Il valore predefinito è false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con caratteri speciali
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visualizza il valore corrente di EncodeEntityAsCode
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Imposta EncodeEntityAsCode su true
            options.EncodeEntityAsCode = true;

            // Salva con le entità codificate come codice
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Imposta EncodeEntityAsCode su false
            options.EncodeEntityAsCode = false;

            // Salva con le entità così come sono
            workbook.Save("HtmlWithRawEntities.html", options);

            // Confronta i file di output
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


