---
title: "BorderCollection.SetColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo BorderCollection. Imposta il Color di tutti i bordi nella collezione"
type: docs
url: /it/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Imposta il Color di tutti i bordi nella raccolta.

```csharp
public void SetColor(Color color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Color dei Borders. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con bordi colorati
            Style style = workbook.CreateStyle();
            
            // Imposta gli stili delle linee di bordo
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Imposta il colore del bordo su rosso usando il metodo SetColor
            style.Borders.SetColor(Color.Red);

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Adatta automaticamente la colonna per una migliore visibilità
            worksheet.AutoFitColumn(0);

            // Salva la cartella di lavoro
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


