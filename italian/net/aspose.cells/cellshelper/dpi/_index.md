---
title: "CellsHelper.DPI"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene il DPI della macchina"
type: docs
url: /it/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Ottiene i DPI della macchina.

```csharp
public static double DPI { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Imposta e visualizza il DPI corrente
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // Modifica l'impostazione DPI
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Crea una nuova cartella di lavoro e salva con impostazioni DPI diverse
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi una forma di esempio per dimostrare l'effetto DPI
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Salva con l'impostazione DPI corrente
            workbook.Save("output_with_dpi_300.xlsx");

            // Modifica il DPI e salva di nuovo
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


