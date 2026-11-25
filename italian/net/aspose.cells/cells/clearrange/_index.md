---
title: "Cells.ClearRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Cancella il contenuto e la formattazione di un intervallo"
type: docs
url: /it/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Cancella il contenuto e la formattazione di un range.

```csharp
public void ClearRange(CellArea range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | CellArea | Intervallo da cancellare. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola le celle con dati di esempio
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Definisci il CellArea da cancellare (righe 0-2, colonne 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Cancella l'intervallo specificato
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Cancella il contenuto e la formattazione di un range.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endRow | Int32 | Indice della riga finale. |
| endColumn | Int32 | Indice della colonna finale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Popola alcuni dati di test
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Cancella l'intero intervallo del foglio di lavoro
            cells.ClearRange(0, 0, 1048575, 16383);

            // Salva la cartella di lavoro
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


