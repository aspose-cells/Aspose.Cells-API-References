---
title: "ListObject.Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-metod. Filtrera tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filtrera tabellen.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd i stället ListObject.HasAutoFilter-egenskapen./// Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för listobjektet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Skapa ett listobjekt från dataområdet med ListObjects.Add med korrekta parametrar
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Hämta AutoFilter via Filter-metoden
                AutoFilter autoFilter = listObject.Filter();

                // Applicera filter på Price-kolumnen (index 1) för att visa poster ≥ 800
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


