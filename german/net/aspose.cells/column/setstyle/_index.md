---
title: "Column.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Methode. Legt die Formatierung dieser Spalte fest"
type: docs
url: /de/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Legt den Stil dieser Spalte fest.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | die Formatierung, die als Standardformatierung für Zellen in dieser Spalte verwendet wird. |

### Hinweise

Diese Methode legt die angegebene Formatierung nur als Standardformatierung für diese Spalte fest, ohne die Formatierungseinstellungen für bereits vorhandene Zellen in dieser Spalte zu ändern. Um die Formatierungseinstellungen vorhandener Zellen gleichzeitig auf die angegebene Formatierung zu aktualisieren, verwenden Sie bitte [`ApplyStyle`](../applystyle/).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die erste Spalte zu
            Column column = worksheet.Cells.Columns[0];

            // Neue Formatierung aus der Arbeitsmappe erstellen
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Die benutzerdefinierte Formatierung auf die gesamte Spalte anwenden
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


