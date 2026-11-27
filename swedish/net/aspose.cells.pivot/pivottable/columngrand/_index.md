---
title: "PivotTable.ColumnGrand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable-rapporten visar totalsummor för kolumner"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/columngrand/
---
## PivotTable.ColumnGrand property

Anger om PivotTable-rapporten visar totalsummor för kolumner.

```csharp
[Obsolete("Use PivotTable.ShowColumnGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ColumnGrand { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowColumnGrandTotals method. Denna metod kommer att tas bort 12 månader senare sedan december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyColumnGrandDemo
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
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Visa det aktuella värdet av ColumnGrand
            Console.WriteLine("Current ColumnGrand value: " + pivotTable.ColumnGrand);

            // Ändra ColumnGrand property
            pivotTable.ColumnGrand = false;

            // Beräkna data för att se effekten
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableColumnGrandDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


