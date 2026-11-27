---
title: "PivotTable.ShowInTabularForm"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Formaterar PivotTable i tabellform"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Formaterar pivottabellen i tabellform.

```csharp
public void ShowInTabularForm()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till dataarbetsblad
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Lägg till exempeldata för pivottabell
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Lägg till pivottabellark
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Lägg till pivottabell
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Lägg till fält i pivottabell
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Visa pivottabell i tabellformat
            pivotTable.ShowInTabularForm();
            
            // Uppdatera och beräkna pivottabellsdata
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


