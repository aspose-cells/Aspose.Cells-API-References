---
title: "Enum BorderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.BorderType. Elenca i tipi di linea di bordo e di linea diagonale"
type: docs
url: /it/net/aspose.cells/bordertype/
---
## BorderType enumeration

Enumera i tipi di linee di bordo e di linee diagonali.

```csharp
[Flags]
public enum BorderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LeftBorder | `1` | Rappresenta la linea del bordo sinistro. |
| RightBorder | `2` | Rappresenta la linea del bordo destro esiste. |
| TopBorder | `4` | Rappresenta la linea del bordo superiore. |
| BottomBorder | `8` | Rappresenta la linea del bordo inferiore. |
| DiagonalDown | `10` | Rappresenta la linea diagonale dall'angolo superiore sinistro a quello inferiore destro. |
| DiagonalUp | `20` | Rappresenta la linea diagonale dall'angolo inferiore sinistro a quello superiore destro. |
| Vertical | `40` | Solo per stile dinamico, come formattazione condizionale, tabella pivot. |
| Horizontal | `80` | Solo per stile dinamico, come formattazione condizionale, tabella pivot. |
| SideBorders | `F` | Indica i quattro bordi laterali: LeftBorder, RightBorder, TopBorder e BottomBorder. |
| Diagonal | `30` | Combinazione speciale di più bordi per comodità dell'utente in alcune API. Indica i bordi diagonali DiagonalUp e DiagonalDown. |
| DynamicStyleBorders | `C0` | Indica verticale e orizzontale per lo stile dinamico. |
| None | `0` | Nessun bordo è stato specificato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Crea un intervallo di celle
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Crea un oggetto stile
            Style style = workbook.CreateStyle();
            // Imposta i bordi per l'intervallo
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Applica lo stile all'intervallo
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Salva la cartella di lavoro
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


