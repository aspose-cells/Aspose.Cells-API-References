---
title: "Cells.ShowGroupDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Espande le righe/colonne raggruppate"
type: docs
url: /it/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Espande le righe/colonne raggruppate.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVertical | Booleano | True, espande le righe raggruppate. |
| indice | Int32 | L'indice di riga/colonna |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati di esempio nelle righe 5-7 (indice basato su zero 4-6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Raggruppa le righe 4-6 (righe Excel 5-7) e comprimile inizialmente
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Espandi le righe raggruppate usando ShowGroupDetail (isVertical: false per le righe, indice: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare l'effetto
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


