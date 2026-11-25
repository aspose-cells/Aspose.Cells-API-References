---
title: "Cells.UnhideColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Mostra più colonne"
type: docs
url: /it/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Rende visibili più colonne.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| totalColumns | Int32 | Numero colonna |
| larghezza | Double | Larghezza colonna. |

### Osservazioni

Applica la larghezza della colonna solo alle colonne nascoste.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Nascondi le colonne 1-3 (indice zero) inizialmente
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Mostra le colonne a partire dall'indice 1 (seconda colonna), larghezza di 3 colonne, imposta la larghezza a 15.5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Verifica le colonne mostrate controllando la loro larghezza
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


