---
title: "OdsPageBackground.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground-egenskap. Hämtar och anger sidbakgrundstypen"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Hämtar och anger sidbakgrundstypen.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladets sidinställning
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Hämta ODS-sidbakgrunden
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Ställ in bakgrundstyp till grafik och konfigurera den
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Spara arbetsboken
            workbook.Save("output.ods");
            
            // Läs in den sparade filen igen för att verifiera inställningarna
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Skriv ut verifieringsresultaten
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Se även

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


