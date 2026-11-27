---
title: "Worksheet.Protection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett kalkylblad. Stöder avancerade skyddsalternativ i ExcelXP och senare versioner"
type: docs
url: /sv/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett arbetsblad. Stöder avancerade skyddsalternativ i ExcelXP och senare versioner.

```csharp
public Protection Protection { get; }
```

### Anmärkningar

Denna egenskap kan skydda kalkylblad i alla versioner av Excel-filer och stödjer avancerade skyddsalternativ i ExcelXP och senare versioner.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Åtkomst till skyddsegenskaper
            Protection protection = sheet.Protection;
            
            // Ställ in skyddsegenskaper
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Skydda kalkylbladet (använd Protect‑metoden istället för att ställa in IsProtectedWithPassword direkt)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Spara arbetsboken
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Verifiera skyddsinställningarna
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Se även

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


