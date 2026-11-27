---
title: "PivotField.CurrentPageItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Hämtar eller anger det för närvarande visade sidobjektet för detta pivåfält, endast sidfältet."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Hämtar eller anger det för närvarande visade sidobjektet för detta pivotfält (endast sidfält).

```csharp
public short CurrentPageItem { get; set; }
```

### Anmärkningar

Use [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) som sentinelvärde för att indikera "Select All". Detta är en fördefinierad markör och är inte ett giltigt objektindex.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Uppdatera data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Hämta sidfält
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Visa aktuella sidobjekt
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Ändra aktuellt sidobjekt
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


