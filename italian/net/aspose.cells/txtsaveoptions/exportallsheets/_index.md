---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se esportare tutti i fogli nel file di testo. Se è false esporta solo il foglio attivo, proprio come MS Excel"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con due fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Aggiungi dati di esempio a entrambi i fogli
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Salva con ExportAllSheets=false (predefinito)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Salva con ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


