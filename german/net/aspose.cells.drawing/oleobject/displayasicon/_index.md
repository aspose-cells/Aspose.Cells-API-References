---
title: "OleObject.DisplayAsIcon"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. True, wenn das angegebene Objekt als Symbol angezeigt wird und das Bild nicht automatisch geändert wird"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True, wenn das angegebene Objekt als Symbol angezeigt wird und das Bild nicht automatisch geändert wird.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein OLE-Objekt (PDF) zum Arbeitsblatt hinzu
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Rufen Sie das OLE-Objekt ab
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Demonstriert die DisplayAsIcon-Eigenschaft
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Inhalt anzeigen, falls möglich
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


