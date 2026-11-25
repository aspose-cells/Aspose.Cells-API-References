---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se i tag HTML come div/div nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indica se i tag HTML (come `<div></div>`) nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio contenenti tag HTML
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il valore della cella con tag HTML
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Crea le opzioni di salvataggio HTML e abilita l'analisi dei tag HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Salva la cartella di lavoro con i tag HTML analizzati
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


