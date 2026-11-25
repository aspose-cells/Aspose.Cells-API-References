---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare solo il foglio di lavoro attivo in un file html. Se true allora solo il foglio di lavoro attivo verrà esportato nel file html. Se false allora l'intera cartella di lavoro verrà esportata nel file html. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indica se esportare solo il foglio di lavoro attivo in un file html. Se true, solo il foglio di lavoro attivo sarà esportato in un file html; se false, l'intera cartella di lavoro sarà esportata in un file html. Il valore predefinito è false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Aggiungi dati di esempio a entrambi i fogli
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Imposta le opzioni di salvataggio HTML per esportare solo il foglio di lavoro attivo
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Imposta il primo foglio di lavoro come attivo
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Salva solo con il foglio di lavoro attivo
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Cambia il foglio attivo e salva di nuovo
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


