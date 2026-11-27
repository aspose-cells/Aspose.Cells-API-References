---
title: "PivotTable.ShowInOutlineForm"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Formaterar PivotTable i konturform"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Formaterar pivottabellen i konturform.

```csharp
public void ShowInOutlineForm()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till arbetsblad med exempeldata
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Lägg till exempeldata
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // Skapa arbetsblad för pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Lägg till pivottabell och hämta referensen
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Visa i konturform
            pivotTable.ShowInOutlineForm();
            
            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


