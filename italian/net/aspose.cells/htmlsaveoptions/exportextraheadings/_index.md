---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare intestazioni extra quando la lunghezza del testo è superiore al massimo della colonna di visualizzazione. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se vuoi importare il file html in Excel, mantieni il valore predefinito.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e intestazioni extra
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Imposta intestazioni extra (righe e colonne)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // Configura le opzioni di salvataggio HTML con ExportExtraHeadings
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // Salva in HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


