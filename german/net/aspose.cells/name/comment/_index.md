---
title: "Name.Comment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt den Kommentar des Namens zurück und legt ihn fest. Gilt nur für Excel 2007 oder neuere Versionen"
type: docs
url: /de/net/aspose.cells/name/comment/
---
## Name.Comment property

Liest und setzt den Kommentar des Namens. Gilt nur für Excel 2007 oder neuere Versionen.

```csharp
public string Comment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen benannten Bereich mit Kommentar hinzufügen
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Speichere die Arbeitsmappe
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Laden Sie die gespeicherte Arbeitsmappe, um den Kommentar zu überprüfen
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Geben Sie den Kommentar aus, um die Funktionalität zu demonstrieren
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


