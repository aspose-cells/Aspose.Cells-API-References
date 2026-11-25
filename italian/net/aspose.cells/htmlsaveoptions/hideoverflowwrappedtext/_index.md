---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta testo di esempio nella cella A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Crea e applica uno stile con a capo automatico del testo
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Ottieni la raccolta di celle e applica lo stile
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Imposta la larghezza della colonna per far avvolgere il testo
            cells.SetColumnWidth(0, 10);
            
            // Crea le opzioni di salvataggio HTML e imposta HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


