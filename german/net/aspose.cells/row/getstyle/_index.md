---
title: "Row.GetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row Methode. Gibt den Stil dieser Zeile zurück"
type: docs
url: /de/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Gibt den Stil dieser Zeile zurück.

```csharp
public Style GetStyle()
```

### Hinweise

Das direkte Ändern des zurückgegebenen Stilobjekts hat keine Wirkung für diese Zeile oder für Zellen in dieser Zeile. Sie müssen die Methode [`ApplyStyle`](../applystyle/) oder [`SetStyle`](../setstyle/) aufrufen, um die Änderung auf diese Zeile anzuwenden. Der Stil der Zeile ist der Stil, der von den Zellen in dieser Zeile geerbt wird (jene Zellen, die keine benutzerdefinierten Stileinstellungen haben, wie bereits vorhandene Zellen, deren Stil nicht explizit gesetzt wurde, oder solche, die noch nicht instanziiert wurden).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Stile für die Demonstration festlegen
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Demonstriere die Verwendung von GetStyle
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

### Siehe auch

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


