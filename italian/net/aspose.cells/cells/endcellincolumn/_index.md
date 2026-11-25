---
title: "Cells.EndCellInColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'ultima cella in questa colonna"
type: docs
url: /it/net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Ottiene l'ultima cella in questa colonna.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |

### Valore di ritorno

Oggetto Cell.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ottieni l'ultima cella nella colonna A (indice colonna 0)
            Cell lastCell = worksheet.Cells.EndCellInColumn(0);
            
            Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);

            // Itera attraverso tutte le righe nella colonna A
            for (int row = 0; row <= lastCell.Row; row++)
            {
                Cell cell = worksheet.Cells[row, 0];
                Console.WriteLine("Row " + row + ": " + cell.StringValue);
            }

            // Salva la cartella di lavoro
            workbook.Save("EndCellInColumnDemo.xlsx");
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

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Ottiene l'ultima cella con indice di colonna massimo in questo intervallo.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati nella colonna B (indice 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Chiama EndCellInColumn con i parametri: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Contrassegna la cella trovata
                    result.PutValue("Last Cell");
                    Style style = result.GetStyle();
                    style.Font.IsBold = true;
                    result.SetStyle(style);
                }
                else
                {
                    Console.WriteLine("No cells found in specified range");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


