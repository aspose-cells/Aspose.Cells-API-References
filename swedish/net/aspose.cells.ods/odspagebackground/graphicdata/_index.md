---
title: "OdsPageBackground.GraphicData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground-egenskap. Hämtar och anger den grafiska datan"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

Hämtar och anger grafikdata.

```csharp
public byte[] GraphicData { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och dess sidinställning
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in ODS-sidbakgrundsegenskaper
            OdsPageBackground background = pageSetup.ODSPageBackground;
            background.Type = OdsPageBackgroundType.Graphic;
            
            // Läs in bilddata och ange som bakgrund
            string imagePath = "sample.png"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                background.GraphicData = File.ReadAllBytes(imagePath);
                background.GraphicType = OdsPageBackgroundGraphicType.Area;
                
                // Spara arbetsboken
                workbook.Save("output.ods");
                
                Console.WriteLine("ODS file with graphic background created successfully.");
            }
            else
            {
                Console.WriteLine("Image file not found: " + imagePath);
            }
        }
    }
}
```

### Se även

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


