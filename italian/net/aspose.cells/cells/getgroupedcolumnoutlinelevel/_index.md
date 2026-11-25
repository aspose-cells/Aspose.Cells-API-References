---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene il livello di contorno a base zero della colonna"
type: docs
url: /it/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Restituisce il livello di contorno (basato su zero) della colonna.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | L'indice di colonna |

### Valore di ritorno

Il livello di contorno della colonna

### Osservazioni

Se la colonna non è raggruppata, restituisce zero.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Raggruppa le colonne (prime 3 colonne) senza nasconderle
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Ottieni il livello di contorno della prima colonna
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


