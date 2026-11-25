---
title: "Row.GetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Ottiene lo stile di questa riga"
type: docs
url: /it/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Ottiene lo stile di questa riga.

```csharp
public Style GetStyle()
```

### Osservazioni

La modifica diretta dell'oggetto stile restituito non ha alcun effetto su questa riga o su qualsiasi cella in essa. È necessario chiamare il metodo [`ApplyStyle`](../applystyle/) o [`SetStyle`](../setstyle/) per applicare la modifica a questa riga. Lo stile della riga è lo stile che verrà ereditato dalle celle in questa riga (quelle celle che non hanno impostazioni di stile personalizzate, come le celle esistenti che non hanno uno stile impostato esplicitamente, o quelle che non sono state istanziate).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta gli stili per la dimostrazione
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Dimostra l'uso di GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


