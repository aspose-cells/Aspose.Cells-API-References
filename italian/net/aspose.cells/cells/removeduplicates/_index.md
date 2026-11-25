---
title: "Cells.RemoveDuplicates"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Rimuove le righe duplicate nel foglio"
type: docs
url: /it/net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Rimuove le righe duplicate nel foglio.

```csharp
public void RemoveDuplicates()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Popola le celle con alcuni valori duplicati
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    // Crea duplicati in ogni altra riga
                    cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
                }
            }

            Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
            
            // Rimuovi i valori duplicati
            cells.RemoveDuplicates();

            Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Rimuove i valori duplicati nell'intervallo.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale. |
| startColumn | Int32 | La colonna iniziale |
| endRow | Int32 | L'indice della riga finale. |
| endColumn | Int32 | L'indice della colonna finale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio con duplicati
            cells["A1"].PutValue("Apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("Apple");
            cells["A4"].PutValue("Banana");
            cells["A5"].PutValue("Orange");

            // Rimuovi i duplicati dalla colonna A (indice basato su zero)
            cells.RemoveDuplicates(0, 0, 5, 0);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Rimuove i dati duplicati dell'intervallo.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale. |
| startColumn | Int32 | La colonna iniziale |
| endRow | Int32 | L'indice della riga finale. |
| endColumn | Int32 | L'indice della colonna finale. |
| hasHeaders | Booleano | Indica se l'intervallo contiene intestazioni. |
| columnOffsets | Int32[] | Gli offset di colonna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola i dati di esempio con duplicati
            cells[0, 0].PutValue("ID");
            cells[0, 1].PutValue("Name");
            cells[0, 2].PutValue("Age");
            
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue("John");
            cells[1, 2].PutValue(30);

            cells[2, 0].PutValue(2);
            cells[2, 1].PutValue("Jane");
            cells[2, 2].PutValue(25);

            cells[3, 0].PutValue(1); // Duplicate ID
            cells[3, 1].PutValue("John"); // Duplicate Name
            cells[3, 2].PutValue(35);

            cells[4, 0].PutValue(3);
            cells[4, 1].PutValue("Bob");
            cells[4, 2].PutValue(40);

            try
            {
                // Rimuovi i duplicati dalle righe 1-4 (indice basato su zero), colonne 0-2
                // Verifica i duplicati basandoti sulle prime due colonne (ID e Nome)
                cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });

                Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("RemoveDuplicatesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


