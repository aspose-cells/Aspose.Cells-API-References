---
title: "Cells.SetRowHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta l'altezza della riga in unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Imposta l'altezza della riga in unità di pollici.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| pollici | Double | Numero di pollici. Deve essere compreso tra 0 e 409,5/72. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta lo stile predefinito
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Imposta altezze delle righe in pollici
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Salva la cartella di lavoro
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


