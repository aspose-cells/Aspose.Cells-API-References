---
title: "WorkbookSettings.BuildVersion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Anger den inkrementella offentliga releasen av applikationen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Anger den inkrementella offentliga releasen av programmet.

```csharp
public string BuildVersion { get; set; }
```

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Ställ in grundinställningar
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Demonstrera BuildVersion-egenskapen
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Spara arbetsboken
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


