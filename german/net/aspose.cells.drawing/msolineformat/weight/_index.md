---
title: "MsoLineFormat.Weight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormat-Eigenschaft. Gibt die Stärke der Linie zurück oder legt sie fest, gemessen in pt"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Gibt das Gewicht der Linie zurück oder setzt es, in pt-Einheiten.

```csharp
public double Weight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Lege den Kommentartext fest
            comment.Note = "Sample comment";
            
            // Greife auf das Zeilenformat der Kommentarform zu und lege die Stärke fest
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfe, ob die Stärke korrekt festgelegt wurde
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Siehe auch

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


