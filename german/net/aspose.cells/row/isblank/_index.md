---
title: "Row.IsBlank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row Eigenschaft. Gibt an, ob die Zeile Daten enthält"
type: docs
url: /de/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Gibt an, ob die Zeile Daten enthält

```csharp
public bool IsBlank { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erhalte die erste Zeile (zunächst leer)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // Daten zur ersten Zeile hinzufügen
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Erstelle eine weitere leere Zeile
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Vergleiche den Leerstatus der Zeile
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


