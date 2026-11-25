---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene il livello di contorno zero-based della riga"
type: docs
url: /it/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Restituisce il livello di contorno (basato su zero) della riga.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | L'indice della riga. |

### Valore di ritorno

Il livello di contorno (zero-based) della riga.

### Osservazioni

Se la riga non è raggruppata, restituisce zero.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Raggruppa le righe 0-3 (livello 1)
            cells.GroupRows(0, 3, false);
            
            // Raggruppa le righe 0-1 (livello 2)
            cells.GroupRows(0, 1, false);

            // Ottieni il livello di contorno per ogni riga
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Annulla il raggruppamento di tutte le righe
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


