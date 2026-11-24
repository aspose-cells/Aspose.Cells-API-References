---
title: "Column.GetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Methode. Gibt den Stil dieser Spalte zurück"
type: docs
url: /de/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Ermittelt den Stil dieser Spalte.

```csharp
public Style GetStyle()
```

### Hinweise

Das direkte Ändern des zurückgegebenen Stilobjekts hat keine Wirkung für diese Spalte oder die Zellen in dieser Spalte. Sie müssen die Methode [`ApplyStyle`](../applystyle/) oder [`SetStyle`](../setstyle/) aufrufen, um die Änderung auf diese Spalte anzuwenden. Der Stil der Spalte ist der Stil, der von den Zellen in dieser Spalte geerbt wird (jene Zellen, die keine benutzerdefinierten Stileinstellungen haben, wie vorhandene Zellen, denen kein Stil explizit zugewiesen wurde, oder solche, die nicht instanziiert wurden).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Stil für Spalte 5 festlegen
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Stil für Zeile 7 festlegen
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Spaltenstil überprüfen
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Zeilenstil überprüfen
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


