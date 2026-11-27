---
title: "Metered.IsMeteredLicensed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered method. Kontrollera om metered är licensierad"
type: docs
url: /sv/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Kontrollera om metered är licensierad

```csharp
public static bool IsMeteredLicensed()
```

### Returvärde

Sant eller falskt

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en Metered-instans
            Metered metered = new Metered();

            try
            {
                // Kontrollera om metered-licensen har tillämpats
                bool isLicensed = Metered.IsMeteredLicensed();

                // Visa resultatet
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Lägg till resultatet i kalkylbladet
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


