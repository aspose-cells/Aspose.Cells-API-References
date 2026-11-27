---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Fönstrets bredd i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

Fönstrets bredd, i enheten centimeter.

```csharp
public double WindowWidthCM { get; set; }
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Ställ in WindowWidthCM-egenskapen (20,32 cm = ~8 tum)
            settings.WindowWidthCM = 20.32;
            
            // Verifiera inställningen genom att skriva ut den
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Spara arbetsboken
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


