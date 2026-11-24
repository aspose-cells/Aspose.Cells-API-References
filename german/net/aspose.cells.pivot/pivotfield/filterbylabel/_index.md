---
title: "PivotField.FilterByLabel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Filtert nach Beschriftungen von Zeilen- oder Spalten-Pivot-Feldern"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfelds.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | PivotFilterType | Der Typ der zu filternden Daten. |
| label1 | String | Die Bezeichnung der Filterbedingung |
| label2 | String | Die obere Begrenzungsbezeichnung der Zwischenfilterbedingung |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Erstelle eine Pivot-Tabelle mit den richtigen Parametern
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Hole das Pivot-Feld
            PivotField field = pivot.RowFields[0];
            
            // Filter anwenden
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


