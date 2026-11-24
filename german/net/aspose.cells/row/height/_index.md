---
title: "Row.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt die Zeilenhöhe zurück und legt sie in der Einheit Punkte fest"
type: docs
url: /de/net/aspose.cells/row/height/
---
## Row.Height property

Liest und setzt die Zeilenhöhe in Punkten.

```csharp
public double Height { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Zeilenhöhe für die erste Zeile
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Füge der Zeile einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Überprüfe und zeige die Zeilenhöhe an
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


