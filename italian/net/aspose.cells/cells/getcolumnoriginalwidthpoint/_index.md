---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'altezza originale della colonna in unità di punto se la colonna è nascosta"
type: docs
url: /it/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Ottiene l'altezza originale della colonna in unità di punto se la colonna è nascosta

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice della riga. |

### Valore di ritorno

Larghezza della colonna nella visualizzazione normale.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Prepara il parametro indice della colonna
            int columnIndex = 0;

            try
            {
                // Ottieni la larghezza originale della colonna in punti
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Modifica la larghezza della colonna
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Ottieni nuovamente la larghezza originale per dimostrare che rimane invariata
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Ottieni la larghezza corrente per mostrare la modifica
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


