---
title: "PivotField.RegionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger regionen för pivottabellen där detta fält visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Anger regionen i pivottabellen där detta fält visas.

```csharp
public PivotFieldType RegionType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hämta det första pivottfältet
            PivotField pivotField = pivotTable.RowFields[0];

            // Visa det aktuella RegionType‑värdet
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // Demonstrera hur man använder RegionType‑egenskapen
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Spara arbetsboken
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


