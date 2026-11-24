---
title: "OleObject.ObjectData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Stellt eingebettete OLE-Objektdaten als Byte-Array dar"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Stellt eingebettete OleObject-Daten als Byte-Array dar.

```csharp
public byte[] ObjectData { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            var workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            var worksheet = workbook.Worksheets[0];
            
            // Beispiel-Dateipfade (ersetze sie durch tatsächliche Pfade in deiner Umgebung)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Füge OLE-Objekt mit initialen Bilddaten hinzu
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Ändere die Daten des OLE-Objekts
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


