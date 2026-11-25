---
title: "Classe Border"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Border. Incapsula l'oggetto che rappresenta il bordo della cella"
type: docs
url: /it/net/aspose.cells/border/
---
## Border class

Incapsula l'oggetto che rappresenta il bordo della cella.

```csharp
public class Border
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Ottiene e imposta il colore con un valore ARGB a 32 bit. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Ottiene o imposta il colore del bordo. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Ottiene o imposta il tipo di bordo della cella. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Ottiene e imposta il colore tematico del bordo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            workbook.Worksheets.Add();

            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedere alla cella "A1" dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];

            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Hello World");

            // Recupero dello stile della cella
            Style style = cell.GetStyle();

            // Impostare lo stile della linea del bordo superiore
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Impostare lo stile della linea del bordo inferiore
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Impostare lo stile della linea del bordo sinistro
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Impostare lo stile della linea del bordo destro
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Applicare lo stile alla cella
            cell.SetStyle(style);

            // Salvataggio del file Excel
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


