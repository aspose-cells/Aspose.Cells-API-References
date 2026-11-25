---
title: "Cells.EndCellInRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'ultima cella in questa riga"
type: docs
url: /it/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Ottiene l'ultima cella in questa riga.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |

### Valore di ritorno

Oggetto Cell.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola i dati nella riga 5 (indice basato su zero)
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // Chiama EndCellInRow con indice di riga 5
                Cell endCell = worksheet.Cells.EndCellInRow(5);
                
                if (endCell != null)
                {
                    Console.WriteLine($"Last cell in row 5: {endCell.Name}");
                    Console.WriteLine($"Cell value: {endCell.StringValue}");
                }
                else
                {
                    Console.WriteLine("No cells found in row 5");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Ottiene l'ultima cella con indice di riga massimo in questo intervallo.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| endRow | Int32 | Indice della riga finale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endColumn | Int32 | Indice della colonna finale. |

### Valore di ritorno

Oggetto Cell.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati nel foglio di lavoro
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // Ottieni la cella finale nella riga 3 tra le colonne 1 e 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // Stampa gli indici di riga e colonna della cella finale
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


