---
title: "Cells.SetColumnWidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale"
type: docs
url: /it/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| pollici | Double | Numero di pollici. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta le larghezze delle colonne in pollici
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Imposta alcuni dati nelle celle per rendere il file visibile
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Salva la cartella di lavoro
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


