---
title: "Worksheet.BackgroundImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar och anger arbetsbladets bakgrundsbild"
type: docs
url: /sv/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Hämtar och anger kalkylbladets bakgrundsbild.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sökväg till bildfilen
            string imagePath = "background.jpg";
            
            // Läs in bildfilen i en byte-array
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Ange bakgrundsbilden för arbetsbladet
            worksheet.BackgroundImage = imageData;
            
            // Spara arbetsboken
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


