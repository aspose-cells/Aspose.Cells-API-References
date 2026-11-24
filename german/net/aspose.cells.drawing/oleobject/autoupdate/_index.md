---
title: "OleObject.AutoUpdate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt an, ob die Verknüpfung zum OleObject automatisch aktualisiert wird oder nicht."
type: docs
url: /de/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Gibt an, ob die Verknüpfung zum OleObject automatisch aktualisiert wird oder nicht.

```csharp
public bool AutoUpdate { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldateien für die Demonstration erstellen
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Beispielbilddatei erstellen, falls sie nicht existiert
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Beispiel-Excel-Datei erstellen, falls sie nicht existiert
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Bilddaten lesen
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // OleObject zum Arbeitsblatt hinzufügen
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // OleObject-Eigenschaften festlegen
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // AutoUpdate-Eigenschaft demonstrieren
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


