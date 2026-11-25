---
title: "Worksheet.PageSetup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta la descrizione dell'impostazione di pagina in questo foglio"
type: docs
url: /it/net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Rappresenta la descrizione dell'impostazione della pagina in questo foglio.

```csharp
public PageSetup PageSetup { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta le proprietà di configurazione della pagina
            worksheet.PageSetup.PrintArea = "A1:L50";
            worksheet.PageSetup.PrintTitleRows = "1:2";
            worksheet.PageSetup.PrintTitleColumns = "A:B";
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetupDemo.xlsx");
            
            Console.WriteLine("Worksheet page setup demo completed successfully.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


