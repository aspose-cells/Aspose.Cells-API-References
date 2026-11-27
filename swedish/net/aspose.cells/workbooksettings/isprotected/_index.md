---
title: "WorkbookSettings.IsProtected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar ett värde som indikerar om strukturen eller fönstret i arbetsboken är skyddat"
type: docs
url: /sv/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Hämtar ett värde som indikerar om strukturen eller fönstret i arbetsboken är skyddat.

```csharp
public bool IsProtected { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;
            
            // Kontrollera om arbetsboken är skyddad
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Skydda arbetsboken med ett lösenord
            settings.Password = "password123";
            
            // Verifiera skyddstatus
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Spara den skyddade arbetsboken
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Öppna den skyddade arbetsboken
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Kontrollera skyddsstatus för den laddade arbetsboken
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


