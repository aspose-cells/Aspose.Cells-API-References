---
title: "PivotConditionalFormat.AddFieldArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotConditionalFormat-metod. Lägger till ett område av pivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Lägger till ett område av pivottfältet.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | PivotFieldType | Regionstypen. |
| fieldName | String | Namnet på pivottfältet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypeStringDemo
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

            // Skapa pivottabell – åtgärdad genom att hämta pivottabellen från indexet
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Lägg till villkorligt format
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Demonstrera AddFieldArea med PivotFieldType- och string-parametrar
            pcf.AddFieldArea(PivotFieldType.Data, "Value");
            pcf.AddFieldArea(PivotFieldType.Row, "Category");

            // Lägg till formatvillkor
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();

            // Beräkna data och spara
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Lägger till ett område av pivottfältet.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | PivotFieldType | Regionstypen. |
| fält | PivotField | Pivottfältet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till fält i pivotområden
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data

            // Lägg till villkorligt format
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            
            // Demonstrera AddFieldArea med PivotFieldType- och PivotField-parametrar
            pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
            
            // Lägg till formatvillkor
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "100";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.Red;

            // Spara arbetsboken
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


