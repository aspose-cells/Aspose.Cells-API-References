---
title: "Worksheet.DisplayRightToLeft"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet‑Eigenschaft. Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false"
type: docs
url: /de/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Stellen Sie die Anzeige von rechts nach links ein
            worksheet.DisplayRightToLeft = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.ods");
            
            // Laden Sie die Arbeitsmappe neu, um die Einstellung zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


