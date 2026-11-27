---
title: "WorkbookSettings.MaxUniqueItemsPerField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar och sätter begränsning av unika objekt per fält"
type: docs
url: /sv/net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

Hämtar och anger begränsningen av unika objekt per fält

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // Visa det aktuella värdet för MaxUniqueItemsPerField
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // Demonstrera att sätta ett nytt värde för MaxUniqueItemsPerField
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // Sätt ett annat värde för att visa att det är ändringsbart
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // Lägg till lite exempeldata för att göra exemplet meningsfullt
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // Spara arbetsboken
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


