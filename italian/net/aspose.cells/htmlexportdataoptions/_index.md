---
title: "Enum HtmlExportDataOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HtmlExportDataOptions. Rappresenta le opzioni per l'esportazione dei dati html"
type: docs
url: /it/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Rappresenta le opzioni per l'esportazione dei dati HTML.

```csharp
public enum HtmlExportDataOptions
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Table | `1` | Esporta il file in html contenente solo la parte della tabella. |
| All | `255` | Esporta tutti i dati in html. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Crea HtmlSaveOptions e imposta HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Modifica HtmlExportDataOptions per esportare solo la parte della tabella
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Salva nuovamente la cartella di lavoro in formato HTML
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


