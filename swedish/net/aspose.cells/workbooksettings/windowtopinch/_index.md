---
title: "WorkbookSettings.WindowTopInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret i enheten tum"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten tum.

```csharp
public double WindowTopInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowTopInch-egenskapen för att placera fönstret 2 tum från toppen
            settings.WindowTopInch = 2.0;

            // Verifiera inställningen genom att skriva ut den
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Spara arbetsboken
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


