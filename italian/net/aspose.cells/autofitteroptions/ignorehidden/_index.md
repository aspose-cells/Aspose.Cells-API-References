---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ignora le righe/colonne nascoste"
type: docs
url: /it/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignora le righe/colonne nascoste.

```csharp
public bool IgnoreHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio e formatta le righe
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Nascondi la riga 1
            worksheet.Cells.Rows[1].IsHidden = true;

            // Crea AutoFitterOptions con IgnoreHidden impostato su true
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Adatta automaticamente le righe ignorando le righe nascoste
            worksheet.AutoFitRows(options);

            // Restituisci le altezze delle righe
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


