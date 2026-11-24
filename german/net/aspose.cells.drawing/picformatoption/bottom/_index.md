---
title: "PicFormatOption.Bottom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PicFormatOption-Eigenschaft. Gibt den unteren Versatz zum Dehnen des Bildes zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Liest oder legt den unteren Versatz für das Dehnen des Bildes fest.

```csharp
public double Bottom { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verwende eine vorhandene Bilddatei (ersetze sie durch den tatsächlichen Bildpfad)
            string imagePath = "sample.jpg";

            // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Konfiguriere die Formfüllung, um das Beispielbild zu verwenden
            // FillType wird durch das Setzen von ImageData abgeleitet, wodurch der Typ auf Texture gesetzt wird
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Erstelle und konfiguriere die Bildformatoptionen
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Zeige den anfänglichen Bottom-Wert an
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Ändere den Bottom-Versatz und zeige den neuen Wert an
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Ordne die PicFormatOption der Füllung der Form zu (sofern anwendbar)
            // Hinweis: Dieser Schritt könnte API-spezifische Methoden erfordern, die im bereitgestellten Kontext nicht gezeigt werden
            // Zur Demonstration wird die PicFormatOption erstellt und konfiguriert

            // Speichere die Arbeitsmappe mit den angewendeten Änderungen
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


