---
title: "TxtSaveOptions.ExportArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. L'intervallo di celle da esportare"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

Intervallo di celle da esportare.

```csharp
public CellArea ExportArea { get; set; }
```

### Osservazioni

Se l'area esportata è stata specificata, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) non avrà effetto.

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola le celle con i dati
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // Configura le opzioni di salvataggio del testo con ExportArea
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Salva solo l'area specificata (prime 3 righe, prime 2 colonne)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


