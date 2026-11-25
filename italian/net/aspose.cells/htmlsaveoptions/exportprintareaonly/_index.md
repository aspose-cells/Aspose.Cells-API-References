---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare solo l'area di stampa nel file html. Il valore predefinito è false."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indica se esportare solo l'area di stampa nel file html. Il valore predefinito è false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Imposta l'area di stampa
            worksheet.PageSetup.PrintArea = "B2:F10";

            // Configura le opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Salva la cartella di lavoro con solo l'area di stampa
            workbook.Save("output.html", options);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


