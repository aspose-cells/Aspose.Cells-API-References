---
title: "PivotField.AutoShowCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt die Anzahl der obersten oder untersten Elemente an, die im angegebenen PivotTable-Feld automatisch angezeigt werden."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

Stellt die Anzahl der obersten oder untersten Elemente dar, die im angegebenen PivotTable‑Feld automatisch angezeigt werden.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.AutoShowCount property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowCount { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.Top10AutoShowSettings.AutoShowCount oder die Methode PivotField.Top10AutoShow(). Diese Methode wird 12 Monate später, ab September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 25;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Zeilenfeld hinzufügen und AutoShow-Eigenschaften festlegen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.AutoShowCount = 2;
            rowField.IsAutoShow = true;
            rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)

            // Daten berechnen und speichern
            pivotTable.CalculateData();
            workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


