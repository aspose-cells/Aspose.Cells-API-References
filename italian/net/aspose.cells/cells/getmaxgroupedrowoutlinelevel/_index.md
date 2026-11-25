---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene il livello di contorno della riga raggruppata massimo (indice zero)"
type: docs
url: /it/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Restituisce il livello di contorno massimo delle righe raggruppate (basato su zero).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Valore di ritorno

Il livello di contorno della riga raggruppata massimo (indice zero)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Raggruppa alcune righe per dimostrare i livelli di contorno
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Aggiungi raggruppamento annidato
            cells.GroupRows(4, 5, true);

            // Ottieni il livello di contorno della riga raggruppata massimo
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Visualizza il risultato
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Visualizza il livello di contorno per ogni riga
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


