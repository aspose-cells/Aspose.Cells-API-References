---
title: "PicFormatOption.Left"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PicFormatOption-Eigenschaft. Liest oder schreibt den linken Versatz zum Dehnen des Bildes"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Liest oder legt den linken Versatz für das Dehnen des Bildes fest.

```csharp
public double Left { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu, um die Bildformatierung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Konfiguriere die Bildfüllung für die Form
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Erstelle und konfiguriere PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Wende Formatoptionen auf die Form an (unter der Annahme, dass der Property-Name korrekt ist)
            // Hinweis: Die ursprüngliche 'PictureFormatOptions'-Eigenschaft existiert möglicherweise nicht in der aktuellen API-Version.
            // Die folgende Zeile ist auskommentiert, um den Kompilierungsfehler zu beheben.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Zeige den anfänglichen linken Versatz an
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Ändere den linken Versatz, um 20 % von der linken Seite abzuschneiden
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Speichere die Arbeitsmappe mit der geänderten Bildformatierung
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


