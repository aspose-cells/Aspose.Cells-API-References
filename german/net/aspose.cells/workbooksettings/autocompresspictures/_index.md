---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen booleschen Wert an, der anzeigt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert"
type: docs
url: /de/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Aktiviere AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Füge ein Beispielbild hinzu, um die Komprimierung zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um die Einstellung zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


