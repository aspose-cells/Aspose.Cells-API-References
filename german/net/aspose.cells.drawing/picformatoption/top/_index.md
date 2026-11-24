---
title: "PicFormatOption.Top"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PicFormatOption-Eigenschaft. Gibt den oberen Versatz zum Dehnen des Bildes zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Liest oder legt den oberen Versatz für das Dehnen des Bildes fest.

```csharp
public double Top { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verwende ein vorhandenes Bild oder gib den korrekten Bildpfad an
            string imagePath = "existingImage.png";

            // Füge eine Form mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Wende Bildfüllung mit ImageData an
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Erstelle und konfiguriere PicFormatOption direkt
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // Angenommen, PicFormatOption muss dem Füllformat zugeordnet werden
            // Dieser Teil könnte eine API-spezifische Implementierung erfordern, die in den Typdefinitionen nicht gezeigt wird
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


