---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Konstruktorn för CustomFilterCollection. Skapar en ny instans"
type: docs
url: /sv/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Skapar en ny instans.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället, vänligen sätt FilterColumn.FilterType till FilterType.CustomFilters och hämta sedan FilterColumn.CustomFilters. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Skapa en ny CustomFilterCollection med hjälp av konstruktorn
                CustomFilterCollection filters = new CustomFilterCollection();

                // Visa standardvärdet för And‑egenskapen
                Console.WriteLine($"Default And property value: {filters.And}");

                // Konstruktorn skapar en tom samling
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Spara arbetsboken
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


