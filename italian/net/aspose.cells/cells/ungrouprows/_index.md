---
title: "Cells.UngroupRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Annulla il raggruppamento delle righe"
type: docs
url: /it/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Separa le righe dal raggruppamento.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima riga da separare. |
| lastIndex | Int32 | L'indice dell'ultima riga da separare. |
| isAll | Booleano | True, rimuove tutte le informazioni raggruppate. Altrimenti, rimuove le informazioni del gruppo esterno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea raggruppamenti di righe nidificati per dimostrazione
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Separa tutti i livelli delle righe 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Separa le righe dal raggruppamento.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima riga da separare. |
| lastIndex | Int32 | L'indice dell'ultima riga da separare. |

### Osservazioni

Rimuove solo le informazioni del gruppo esterno.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Raggruppa le righe da 1 a 3 (indice base 0)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Separa le stesse righe
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Salva la cartella di lavoro
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


