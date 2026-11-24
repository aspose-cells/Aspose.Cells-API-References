---
title: "Worksheet.Hyperlinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die HyperlinkCollection-Sammlung zurück"
type: docs
url: /de/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Gibt die [`HyperlinkCollection`](../../hyperlinkcollection/) Sammlung zurück.

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügt dem Arbeitsblatt einen Hyperlink hinzu
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Lädt die gespeicherte Arbeitsmappe, um den Hyperlink zu überprüfen
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Hyperlink-Adresse anzeigen
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Siehe auch

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


