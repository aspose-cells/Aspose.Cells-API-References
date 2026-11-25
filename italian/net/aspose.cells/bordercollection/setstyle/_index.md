---
title: "BorderCollection.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo BorderCollection. Imposta lo stile di tutti i bordi della collezione"
type: docs
url: /it/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Imposta lo stile di tutti i bordi della raccolta.

```csharp
public void SetStyle(CellBorderType style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | CellBorderType | Stile dei bordi |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la cella C6 e il suo stile
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Imposta il colore e lo stile del bordo
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


