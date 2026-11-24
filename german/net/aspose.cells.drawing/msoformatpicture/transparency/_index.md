---
title: "MsoFormatPicture.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt den Transparenzgrad des Bereichs zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (vollständig transparent)"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt zwei Bilder hinzu
            int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
            int index2 = worksheet.Pictures.Add(2, 0, "image2.png");

            // Setzen Sie die Transparenz für die Bilder
            worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
            worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;

            // Speichern und laden Sie die Arbeitsmappe erneut, um die Transparenzeinstellungen zu überprüfen
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];

            // Geben Sie die Transparenzwerte in der Konsole aus
            Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
            Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


