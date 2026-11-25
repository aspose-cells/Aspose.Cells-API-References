---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indica se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // Imposta le opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Salva con foglio di lavoro nascosto non esportato
            workbook.Save("output_without_hidden.html", saveOptions);

            // Modifica l'opzione per esportare i fogli di lavoro nascosti
            saveOptions.ExportHiddenWorksheet = true;

            // Salva con foglio di lavoro nascosto esportato
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


