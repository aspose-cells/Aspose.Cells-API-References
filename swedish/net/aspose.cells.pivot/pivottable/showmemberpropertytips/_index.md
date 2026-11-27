---
title: "PivotTable.ShowMemberPropertyTips"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om medlems‑egenskapsinformation ska utelämnas från PivotTable‑verktygstips"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showmemberpropertytips/
---
## PivotTable.ShowMemberPropertyTips property

Specificerar ett booleskt värde som anger om medlems‑egenskapsinformation ska utelämnas från PivotTable‑verktygstips.

```csharp
public bool ShowMemberPropertyTips { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowMemberPropertyTipsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella värdet för ShowMemberPropertyTips
            Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);

            // Ändra egenskapen ShowMemberPropertyTips
            pivotTable.ShowMemberPropertyTips = false;
            Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);

            // Beräkna data och uppdatera pivottabellen
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Spara arbetsboken
            workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


