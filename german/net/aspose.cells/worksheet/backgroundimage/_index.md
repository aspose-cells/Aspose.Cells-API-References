---
title: "Worksheet.BackgroundImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt das Hintergrundbild des Arbeitsblatts zurück und legt es fest"
type: docs
url: /de/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Liest und setzt das Hintergrundbild des Arbeitsblatts.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Pfad zur Bilddatei
            string imagePath = "background.jpg";
            
            // Lese die Bilddatei in ein Byte-Array ein
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Legen Sie das Hintergrundbild für das Arbeitsblatt fest
            worksheet.BackgroundImage = imageData;
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


