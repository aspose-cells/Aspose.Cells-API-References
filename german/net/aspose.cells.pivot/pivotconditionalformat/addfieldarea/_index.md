---
title: "PivotConditionalFormat.AddFieldArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotConditionalFormat-Methode. Fügt einen Bereich eines Pivot-Feldes hinzu"
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Fügt einen Bereich eines Pivot‑Feldes hinzu.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | PivotFieldType | Der Regionstyp. |
| fieldName | String | Der Name des Pivotfelds. |

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
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

            // Pivot-Tabelle erstellen – behoben, indem die Pivot-Tabelle über den Index abgerufen wird
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Bedingtes Format hinzufügen
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Demonstrieren Sie AddFieldArea mit PivotFieldType- und String-Parametern
            pcf.AddFieldArea(PivotFieldType.Data, "Value");
            pcf.AddFieldArea(PivotFieldType.Row, "Category");

            // Formatbedingung hinzufügen
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();

            // Daten berechnen und speichern
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Fügt einen Bereich eines Pivot‑Feldes hinzu.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | PivotFieldType | Der Regionstyp. |
| Feld | PivotField | Das Pivotfeld. |

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Fügt Felder zu Pivot-Bereichen hinzu.
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data

            // Bedingtes Format hinzufügen
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            
            // Demonstriere AddFieldArea mit PivotFieldType und PivotField Parametern
            pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
            
            // Formatbedingung hinzufügen
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "100";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


