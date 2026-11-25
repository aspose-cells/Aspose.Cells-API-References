---
title: "Cells.GetColumnWidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene la larghezza della colonna specificata nella vista normale, in unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Ottiene la larghezza della colonna specificata nella vista normale, in unità di pollici.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna |

### Valore di ritorno

Larghezza della colonna

Larghezza della colonna nella visualizzazione normale.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la larghezza della colonna in pollici per la dimostrazione
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Chiama GetColumnWidthInch con parametro Int32
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Visualizza il risultato
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


