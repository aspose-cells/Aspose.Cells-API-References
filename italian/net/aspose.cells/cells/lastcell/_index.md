---
title: "Cells.LastCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene l'ultima cella in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Ottiene l'ultima cella in questo foglio di lavoro.

```csharp
public Cell LastCell { get; }
```

### Osservazioni

Restituisce null se non ci sono dati nel foglio di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Ottieni l'indirizzo dell'ultima cella
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Crea un intervallo dalla prima all'ultima cella
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Applica la formattazione all'intervallo
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Salva la cartella di lavoro
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


