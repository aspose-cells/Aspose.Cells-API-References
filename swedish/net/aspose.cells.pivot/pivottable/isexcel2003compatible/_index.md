---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable. Om true måste en sträng vara högst 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng ingen sådan begränsning. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable; om true måste en sträng vara mindre än eller lika med 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng inte den nämnda begränsningen. Standardvärdet är true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Lägg till rader med exempeldata
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Lägg till en pivottabell
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabellens fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Ställ in kompatibilitetsläge
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


