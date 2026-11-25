---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Indica se esportare il collegamento ipertestuale usando definizioni di riferimento invece del formato inline. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Inserisci un testo di esempio in una cella
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Aggiungi un collegamento ipertestuale alla cella (A1)
            // Parametri: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Inizializza le opzioni di salvataggio Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Accedi direttamente alla proprietà ExportHyperlinkAsReference (sola lettura in questa demo)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Salva la cartella di lavoro come markdown; la proprietà (se true) influenzerà il modo in cui i collegamenti ipertestuali vengono esportati
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


