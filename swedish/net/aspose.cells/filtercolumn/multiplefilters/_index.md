---
title: "FilterColumn.MultipleFilters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskapen. Hämtar MultipleFilterCollection för filtrering av data efter etiketter eller datum/tid"
type: docs
url: /sv/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Hämtar [`MultipleFilterCollection`](../../multiplefiltercollection/) för filtrering av data efter etiketter eller datum/tid.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället FilterColumn.FilterValues-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Tillämpa AutoFilter på intervallet
                worksheet.AutoFilter.Range = "A1:A5";

                // Hämta den första filterkolumnen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Skapa och ange MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Tilldela MultipleFilters till filterkolumnen
                filterColumn.MultipleFilters = multipleFilters;

                // Visa MultipleFilters-egenskaperna
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Spara arbetsboken
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


