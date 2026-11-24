---
title: "Picture.SourceFullName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Gibt den Pfad und Namen der Quelldatei für das verknüpfte Bild zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Liest oder setzt den Pfad und Namen der Quelldatei für das verknüpfte Bild.

```csharp
public string SourceFullName { get; set; }
```

### Hinweise

Der Standardwert ist eine leere Zeichenfolge. Wenn SourceFullName keine leere Zeichenfolge ist, wird das Bild verknüpft. Wenn SourceFullName keine leere Zeichenfolge ist, aber Data null ist, wird das Bild verknüpft und nicht in der Datei gespeichert.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein verknüpftes Bild zum Arbeitsblatt hinzu
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Demonstriere die SourceFullName-Eigenschaft
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


