---
title: "Worksheet.TabId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt den internen Bezeichner für das Blatt an"
type: docs
url: /de/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Gibt den internen Bezeichner für das Blatt an.

```csharp
public int TabId { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die TabId-Eigenschaft
            worksheet.TabId = 107;
            
            // Speichere die Arbeitsmappe
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Lade die gespeicherte Arbeitsmappe, um die TabId zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Zeige den TabId-Wert an
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


