---
title: "Cells.GroupRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Raggruppa le righe"
type: docs
url: /it/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Raggruppa le righe.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima riga da raggruppare. |
| lastIndex | Int32 | L'indice dell'ultima riga da raggruppare. |
| isHidden | Booleano | Specifica se le righe raggruppate sono nascoste. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Raggruppa le righe da 1 a 5 (indice base 0) e nascondile
            cells.GroupRows(1, 5, true);

            // Imposta la riga di riepilogo sotto il gruppo
            worksheet.Outline.SummaryRowBelow = false;

            // Salva la cartella di lavoro
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Raggruppa le righe.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | L'indice della prima riga da raggruppare. |
| lastIndex | Int32 | L'indice dell'ultima riga da raggruppare. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
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
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Raggruppa le righe da 2 a 5 (indice base zero)
            cells.GroupRows(1, 4);

            // Salva la cartella di lavoro
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


