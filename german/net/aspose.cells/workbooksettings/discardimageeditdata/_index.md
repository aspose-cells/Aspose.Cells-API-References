---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob Bildbearbeitungsdaten verworfen werden"
type: docs
url: /de/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Gibt an, ob das Verwerfen von bearbeiteten Bilddaten erfolgt.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Bild zum Arbeitsblatt hinzu
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Setze DiscardImageEditData auf true (Standard ist false)
            workbook.Settings.DiscardImageEditData = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Überprüfe, ob die Einstellung angewendet wurde
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


