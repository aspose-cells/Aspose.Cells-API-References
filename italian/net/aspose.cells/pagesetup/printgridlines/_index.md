---
title: "PageSetup.PrintGridlines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta se le linee della griglia delle celle sono stampate sulla pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Rappresenta se le linee della griglia delle celle vengono stampate sulla pagina.

```csharp
public bool PrintGridlines { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci dati di esempio nella cella
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Attiva/disattiva la proprietà PrintGridlines
            worksheet.PageSetup.PrintGridlines = true;
            
            // Salva la cartella di lavoro
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


