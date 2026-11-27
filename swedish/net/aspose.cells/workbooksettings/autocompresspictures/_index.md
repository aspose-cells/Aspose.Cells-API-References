---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Anger ett booleskt värde som visar att programmet automatiskt komprimerar bilder i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Anger ett booleskt värde som visar att programmet automatiskt komprimerar bilder i arbetsboken.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Aktivera AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Lägg till en exempelbild för att demonstrera komprimering
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera inställningen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


