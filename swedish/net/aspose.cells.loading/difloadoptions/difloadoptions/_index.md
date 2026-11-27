---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DifLoadOptions‑konstruktor. Alternativen"
type: docs
url: /sv/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Alternativen.

```csharp
public DifLoadOptions()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny instans av DifLoadOptions med den parameterlösa konstruktorn
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Skapa en ny arbetsbok med standardalternativ
                Workbook workbook = new Workbook();

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata för att demonstrera att arbetsboken fungerar
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Spara arbetsboken i DIF-format
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Läs nu in den sparade DIF‑filen med DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Spara den inlästa datan till XLSX för verifiering
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


