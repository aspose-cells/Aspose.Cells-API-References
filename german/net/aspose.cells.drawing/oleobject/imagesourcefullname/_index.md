---
title: "OleObject.ImageSourceFullName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt den Pfad und Namen der Quelldatei für das verknüpfte Bild zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Liest oder setzt den Pfad und Namen der Quelldatei für das verknüpfte Bild.

```csharp
public string ImageSourceFullName { get; set; }
```

### Hinweise

Der Standardwert ist eine leere Zeichenfolge. Wenn SourceFullName keine leere Zeichenfolge ist, wird das Bild verknüpft. Wenn SourceFullName keine leere Zeichenfolge ist, aber Data null ist, wird das Bild verknüpft und nicht in der Datei gespeichert.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispiel-PDF-Datei zum Einbetten
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Setzen Sie OleObject-Eigenschaften, einschließlich ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


