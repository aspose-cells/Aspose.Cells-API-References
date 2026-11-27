---
title: "WorkbookSettings.ProtectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar skyddstypen för arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Hämtar skyddstypen för arbetsboken.

```csharp
public ProtectionType ProtectionType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skydda arbetsboken med Windows-skyddstyp
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Demonstrera ProtectionType-egenskapen
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Spara arbetsboken
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera att skyddstypet kvarstår
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Se även

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


