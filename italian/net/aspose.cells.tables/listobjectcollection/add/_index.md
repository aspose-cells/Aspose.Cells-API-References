---
title: "ListObjectCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObjectCollection. Aggiunge un ListObject al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Aggiunge un **ListObject** al foglio di lavoro.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale dell'intervallo dell'elenco. |
| startColumn | Int32 | La riga iniziale dell'intervallo dell'elenco. |
| endRow | Int32 | La riga iniziale dell'intervallo dell'elenco. |
| endColumn | Int32 | La riga iniziale dell'intervallo dell'elenco. |
| hasHeaders | Booleano | Indica se l'intervallo ha intestazioni. |

### Valore di ritorno

L'indice del nuovo ListObject

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati in un intervallo
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Aggiungi ListObject usando il metodo Add con parametri Int32
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Abilita i totali e imposta la formula per una colonna
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Salva la cartella di lavoro
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Aggiunge un **ListObject** al foglio di lavoro.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCell | String | La cella iniziale dell'intervallo dell'elenco. |
| endCell | String | La cella finale dell'intervallo dell'elenco. |
| hasHeaders | Booleano | Indica se l'intervallo ha intestazioni. |

### Valore di ritorno

L'indice del nuovo ListObject

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Aggiungi ListObject usando riferimenti di intervallo stringa
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


