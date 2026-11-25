---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta la larghezza della colonna in diverse visualizzazioni"
type: docs
url: /it/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Imposta la larghezza della colonna in visualizzazioni diverse.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice della colonna. |
| pixel | Int32 | La larghezza in unità di pixel. |

### Osservazioni

Se il tipo di visualizzazione corrente è PageLayoutView, la larghezza della colonna è la stessa della larghezza stampata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Imposta dati di esempio
            sheet.Cells[0, 0].Value = "Sample Text";

            // Calcola la larghezza in pixel (100 pixel in questo esempio)
            int pixelWidth = 100;

            // Imposta la larghezza della colonna in pixel
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


