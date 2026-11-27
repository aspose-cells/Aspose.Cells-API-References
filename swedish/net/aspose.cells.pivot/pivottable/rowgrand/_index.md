---
title: "PivotTable.RowGrand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om sammanlagda totaler för rader i den här pivottabellen ska visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Anger om sammanlagda totaler för rader i den här pivottabellen ska visas.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd i stället PivotTable.ShowRowGrandTotals-metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet för RowGrand
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // Ändra RowGrand-egenskapen
            pivotTable.RowGrand = false;

            // Beräkna pivottabellsdata
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


