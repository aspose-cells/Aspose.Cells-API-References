---
title: "WorkbookSettings.WindowTop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret i enheten punkt"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten punkt.

```csharp
public double WindowTop { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowTop-egenskapen för att placera fönstret 100 pixlar från toppen
            settings.WindowTop = 100;
            
            // Verifiera WindowTop-värdet
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Spara arbetsboken
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


