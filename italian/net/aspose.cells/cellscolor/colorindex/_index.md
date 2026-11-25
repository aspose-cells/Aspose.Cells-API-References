---
title: "CellsColor.ColorIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Ottiene e imposta l'indice di colore nella tavolozza dei colori. Si applica solo ai colori indicizzati"
type: docs
url: /it/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Ottiene e imposta l'indice del colore nella tavolozza dei colori. Si applica solo ai colori indicizzati.

```csharp
public int ColorIndex { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definisci un intervallo al quale applicheremo un bordo colorato
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Crea un'istanza di CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Imposta il ColorIndex (indice della tavolozza) – ad esempio, 5
            cellsColor.ColorIndex = 5;

            // Applica CellsColor come colore del bordo interno dell'intervallo
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Leggi e visualizza il valore corrente di ColorIndex
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Salva la cartella di lavoro per visualizzare il risultato
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


