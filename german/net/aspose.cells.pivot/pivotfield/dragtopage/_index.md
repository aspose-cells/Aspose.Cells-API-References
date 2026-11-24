---
title: "PivotField.DragToPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowDraggingToPage. Diese Methode wird 12 Monate nach Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Felder hinzufügen und DragToPage konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // DragToPage-Eigenschaft demonstrieren
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot-Tabelle aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Arbeitsmappe speichern.
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


