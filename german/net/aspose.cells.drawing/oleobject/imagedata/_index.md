---
title: "OleObject.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Stellt das Bild des Ole-Objekts als Byte-Array dar"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Stellt das Bild des OleObject als Byte-Array dar.

```csharp
public byte[] ImageData { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Bilddatei in Byte-Array einlesen
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // OLE-Objekt mit den Bilddaten hinzufügen
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Eingebettete Objekt‑Eigenschaften festlegen
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Verwendung der ImageData-Eigenschaft demonstrieren
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


