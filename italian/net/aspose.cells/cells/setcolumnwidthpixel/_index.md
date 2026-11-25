---
title: "Cells.SetColumnWidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale"
type: docs
url: /it/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| pixel | Int32 | Numero di pixel. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta le larghezze delle colonne in pixel per le colonne da 1 a 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Salva la cartella di lavoro
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


