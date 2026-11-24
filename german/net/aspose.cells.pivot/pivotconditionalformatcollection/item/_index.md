---
title: "PivotConditionalFormatCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotConditionalFormatCollection-Eigenschaft. Gibt das pivot FormatCondition-Objekt am angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

Liefert das Pivot FormatCondition-Objekt am angegebenen Index.

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### Rückgabewert

pivot FormatCondition-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Bedingtes Format hinzufügen
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
            pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });

            // Formatbedingung hinzufügen
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "90";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Pivot-Tabelle berechnen und speichern
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


