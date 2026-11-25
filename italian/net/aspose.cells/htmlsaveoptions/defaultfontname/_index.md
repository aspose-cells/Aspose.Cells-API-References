---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Specifica il nome del font predefinito per l'esportazione in html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale. Il valore predefinito è null."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Specifica il nome del font predefinito per l'esportazione html, il font predefinito verrà utilizzato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale, il valore predefinito è null.

```csharp
public string DefaultFontName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Imposta le opzioni di salvataggio HTML con un font predefinito personalizzato
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // Salva in HTML con il font specificato
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


