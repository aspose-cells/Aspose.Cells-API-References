---
title: "Cells.ClearContents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Cancella il contenuto di un intervallo"
type: docs
url: /it/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Cancella il contenuto di un range.

```csharp
public void ClearContents(CellArea range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | CellArea | Intervallo da cancellare. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola alcuni dati in un'area di celle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Cancella il contenuto dell'area di celle
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
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

## ClearContents(int, int, int, int) {#clearcontents_1}

Cancella il contenuto di un range.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcune celle con valori
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Mostra i valori originali
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Cancella il contenuto delle celle nell'intervallo (0,1) a (1,1)
            cells.ClearContents(0, 1, 1, 1);

            // Mostra i valori dopo la cancellazione
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Salva la cartella di lavoro
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


