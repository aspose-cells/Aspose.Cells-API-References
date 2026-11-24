---
title: "PivotField.DragToHide"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob dieses Pivot-Feld aus der PivotTable-Ansicht entfernt werden kann. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/dragtohide/
---
## PivotField.DragToHide property

Gibt an, ob dieses Pivot-Feld aus der PivotTable-Ansicht entfernt werden kann. Der Standardwert ist true.

```csharp
[Obsolete("Use PivotField.AllowRemovingFromView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToHide { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.AllowRemovingFromView. Diese Methode wird 12 Monate später ab Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToHideDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;
            cells["B5"].Value = 250;

            // Pivot-Tabelle erstellen – Index zuerst ermitteln, dann das PivotTable-Objekt abrufen
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen und DragToHide konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToHide = true; // Core demonstration of the property
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot-Tabelle aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldDragToHideDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


