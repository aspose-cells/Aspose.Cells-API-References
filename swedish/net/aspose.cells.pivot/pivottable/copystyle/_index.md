---
title: "PivotTable.CopyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Kopierar namngiven stil från en annan pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Kopierar namngiven stil från en annan pivottabell.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | PivotTable | Källpivottabell. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Skapa källarbok med pivottabell
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Lägg till exempeldata
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Skapa källpivottabell (hämta explicit pivottabellobjektet)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Tillämpa stil på källpivottabell
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Skapa destinationsarbok med pivottabell
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Lägg till samma datastruktur
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Skapa destinationspivottabell (hämta explicit pivottabellobjektet)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Kopiera stil från källpivottabell till destinationspivottabell
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Spara resultatet
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


