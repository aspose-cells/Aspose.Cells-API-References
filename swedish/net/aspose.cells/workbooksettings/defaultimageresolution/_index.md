---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar och anger standardupplösning för bild"
type: docs
url: /sv/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Hämtar och anger standardupplösning för bild.

```csharp
public int DefaultImageResolution { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange standardupplösning för bild
            workbook.Settings.DefaultImageResolution = 300;
            
            // Lägg till ett kalkylblad och infoga en bild
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera standardupplösning för bild
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


