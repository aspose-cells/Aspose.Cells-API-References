---
title: "PivotTable.GrandTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Returnerar etiketten som visas i rubriken för totalraden eller -kolumnen. Standardvärdet är strängen Grand Total"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Returnerar etiketten som visas i rubriken för total‑kolumnen eller -raden. Standardvärdet är strängen "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visa det aktuella GrandTotalName-värdet
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // Ändra GrandTotalName
            pivotTable.GrandTotalName = "Total Summary";

            // Beräkna data och uppdatera pivottabellen
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Spara arbetsboken
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


