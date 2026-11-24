---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFormatPicture-Eigenschaft. Gibt an, ob dieses Bild in zweifarbigen Schwarz‑Weiß angezeigt werden soll"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Gibt an, ob dieses Bild in zweifarbigen Schwarz‑Weiß angezeigt werden soll.

```csharp
public bool IsBiLevel { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein Bild zum Arbeitsblatt hinzufügen
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Setzen Sie das Bild auf zweifarbige Darstellung (Schwarz‑Weiß)
            picture.FormatPicture.IsBiLevel = true;
            
            // Überprüfen und ausgeben Sie den Wert der IsBiLevel-Eigenschaft
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


