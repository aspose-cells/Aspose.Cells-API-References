---
title: "PivotConditionalFormat.ApplyTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotConditionalFormat-metod. Tillämpar det villkorliga formatet på ett område som måste ligga i datasegmentet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/applyto/
---
## PivotConditionalFormat.ApplyTo method

Tillämpar det villkorliga formatet på ett område som måste vara i dataregionen.

```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Den valda raden. |
| column | Int32 | Den valda kolumnen. |
| omfång | PivotConditionFormatScopeType | Omfånget |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodApplyToWithInt32Int32PivotConditionFormatDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotTableIndex];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Lägg till villkorligt format
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            
            // Demonstrera ApplyTo-metoden med specifika parametrar
            pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
            
            // Lägg till formatvillkor
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
            
            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


