---
title: "Cells.DeleteRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina più righe"
type: docs
url: /it/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Elimina più righe.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | L'indice della prima riga da eliminare. |
| totalRows | Int32 | Numero di righe da eliminare. |

### Osservazioni

Se l'intervallo eliminato contiene la parte superiore (non l'intero) della tabella (ListObject), l'intervallo non può essere eliminato e non verrà eseguita alcuna operazione. Funziona allo stesso modo di MS Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Elimina 2 righe a partire dall'indice riga 2 (3ª riga)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Elimina più righe nel foglio di lavoro.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della prima riga da eliminare. |
| totalRows | Int32 | Numero di righe da eliminare. |
| updateReference | Booleano | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importa dati nelle celle
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Crea una tabella
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Elimina la riga all'indice 1 (seconda riga) aggiornando i riferimenti
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Elimina più righe nel foglio di lavoro.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della prima riga da eliminare. |
| totalRows | Int32 | Numero di righe da eliminare. |
| opzioni | DeleteOptions | Opzioni per l'operazione di eliminazione |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta dati di esempio e formule
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Elimina la riga 2 senza monitoraggio (poiché FormulaChangeMonitor non è disponibile)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### Vedi anche

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


