---
title: "PivotTable.IsMultipleFieldFilters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/ismultiplefieldfilters/
---
## PivotTable.IsMultipleFieldFilters property

Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem.

```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.AllowMultipleFiltersPerField-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyIsMultipleFieldFiltersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("Fruit");
            worksheet.Cells["B3"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue("Fruit");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet av IsMultipleFieldFilters
            Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);

            // Ställ in IsMultipleFieldFilters till true för att tillåta flera filter per fält
            pivotTable.IsMultipleFieldFilters = true;
            Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);

            // Uppdatera och beräkna pivottabellen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


