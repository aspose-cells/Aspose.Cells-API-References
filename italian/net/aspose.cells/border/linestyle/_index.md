---
title: "Border.LineStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Border. Ottiene o imposta il tipo di bordo della cella"
type: docs
url: /it/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Ottiene o imposta il tipo di bordo della cella.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a una cella e ottieni il suo stile
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Imposta diversi stili di linea del bordo
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


