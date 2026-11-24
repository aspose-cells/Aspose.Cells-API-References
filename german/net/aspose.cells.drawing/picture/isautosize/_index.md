---
title: "Picture.IsAutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. True gibt an, dass die Größe des OLE-Objekts automatisch geändert wird, wenn die Größe des Schnappschusses des eingebetteten Inhalts beim Aktivieren des OLE-Objekts angepasst wird."
type: docs
url: /de/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

True zeigt an, dass die Größe des OLE-Objekts automatisch geändert wird, entsprechend der Größe des Schnappschusses des eingebetteten Inhalts, wenn das OLE-Objekt aktiviert wird.

```csharp
public bool IsAutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Demonstriere die IsAutoSize-Eigenschaft
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Setze IsAutoSize auf true - das Bild wird automatisch an den Inhalt angepasst
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Setze IsAutoSize auf false - das Bild behält seine ursprünglichen Abmessungen bei
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Speichere die Arbeitsmappe
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


