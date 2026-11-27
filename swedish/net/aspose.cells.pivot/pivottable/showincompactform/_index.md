---
title: "PivotTable.ShowInCompactForm"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Layoutar pivottabellvyn i kompakt form"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Formaterar pivottabellvyn i kompakt form.

```csharp
public void ShowInCompactForm()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från källdata
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Skapa ett pivottabellark
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Lägg till pivottabell
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ställ in pivottabellen så att den visas i kompakt form
            pivotTable.ShowInCompactForm();
            
            // Beräkna data och uppdatera
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


