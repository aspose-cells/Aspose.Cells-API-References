---
title: "Worksheet.Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Filtra l'intervallo"
type: docs
url: /it/net/aspose.cells/worksheet/filter/
---
## Worksheet.Filter method

Filtra l'intervallo.

```csharp
public void Filter(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class WorksheetMethodFilterWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio (inclusa una riga di intestazione)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            try
            {
                // Definisci l'intervallo a cui verrà applicato il filtro
                CellArea filterArea = new CellArea
                {
                    StartRow = 0,      // Row 1 (zero‑based)
                    StartColumn = 0,   // Column A
                    EndRow = 4,        // Row 5
                    EndColumn = 1      // Column B
                };

                // Applica un filtro automatico all'area definita
                worksheet.Filter(filterArea);

                // Salva la cartella di lavoro per verificare che il filtro sia stato impostato
                workbook.Save("WorksheetFilterWithCellAreaDemo.xlsx");

                Console.WriteLine("Filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


