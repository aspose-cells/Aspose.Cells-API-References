---
title: "Column.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt die Spaltenbreite in Zeichen zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/column/width/
---
## Column.Width property

Ermittelt und legt die Spaltenbreite in Zeichen als Einheit fest.

```csharp
public double Width { get; set; }
```

### Hinweise

Bei Tabellenkalkulationen wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Breite für Spalte 3 (Index 2) festlegen
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Breite für Spalte 4 (Index 3) festlegen
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Breiten abrufen und anzeigen
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


