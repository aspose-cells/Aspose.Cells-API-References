---
title: "Protection.AllowEditingScenario"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection egenskap. Anger om användaren får redigera scenarier på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Representerar om användaren får redigera scenarier på ett skyddat kalkylblad.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Åtkomst till arbetsbladsskyddinställningar
            Protection protection = worksheet.Protection;

            // Ställ in skyddsegenskaper med AllowEditingScenario aktiverat
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Skydda kalkylbladet
            worksheet.Protect(ProtectionType.All);

            // Spara arbetsboken
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


