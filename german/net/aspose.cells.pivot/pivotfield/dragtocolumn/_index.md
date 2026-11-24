---
title: "PivotField.DragToColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Eigenschaft. Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToColumn property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToColumn { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.AllowDraggingToColumn‑Eigenschaft. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToColumnDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Item");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(8);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Rufen Sie das Datenfeld ab und setzen Sie DragToColumn auf true.
            PivotField quantityField = pivotTable.DataFields[0];
            quantityField.DragToColumn = true; // This allows the field to be dragged to column area
            quantityField.DisplayName = "Total Quantity";

            // Daten berechnen und speichern
            pivotTable.CalculateData();
            workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


