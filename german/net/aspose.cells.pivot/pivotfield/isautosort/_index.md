---
title: "PivotField.IsAutoSort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob die Elemente dieses PivotTable-Feldes automatisch sortiert werden"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Gibt an, ob die Elemente dieses PivotTable-Feldes automatisch sortiert werden.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoSort { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.SortSetting.SortType‑Eigenschaft oder die PivotField.SortBy()-Methode. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSortDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Blueberry";
            cells["B5"].Value = 15;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Zeilenfeld hinzufügen und automatische Sortierung festlegen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsAutoSort = true;
            rowField.AutoSortField = 1; // Sort by Quantity (column B)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldIsAutoSortDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


