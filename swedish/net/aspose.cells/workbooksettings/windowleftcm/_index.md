---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Avståndet från den vänstra kanten av klientområdet till den vänstra kanten av fönstret. I centimeter"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten centimeter.

```csharp
public double WindowLeftCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowLeftCM-egenskapen (avstånd från skärmens vänstra kant i centimeter)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Verifiera inställningen genom att skriva ut den
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Spara arbetsboken
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


