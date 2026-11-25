---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene il livello di contorno della colonna raggruppata massimo (basato su zero)"
type: docs
url: /it/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Restituisce il livello di contorno massimo delle colonne raggruppate (basato su zero).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Valore di ritorno

Il livello di contorno della colonna raggruppata massimo (basato su zero)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Raggruppa alcune colonne per dimostrare i livelli di contorno
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Ottieni il livello di contorno della colonna raggruppata massimo
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Visualizza il livello di contorno per ogni colonna
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


