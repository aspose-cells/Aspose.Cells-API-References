---
title: "PivotFilter.Value1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Eigenschaft. Gibt den Zeichenkettenwert1 des Beschriftungs‑Pivotfilters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

Ermittelt den Zeichenkettenwert1 des Beschriftungs-Pivotfilters.

```csharp
public string Value1 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Arbeitsblatt mit Beispieldaten füllen
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Fügen Sie eine Pivot-Tabelle hinzu
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Fügen Sie einen Pivot‑Filter hinzu und setzen Sie Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // Aktualisieren und Daten berechnen
            pivot.RefreshData();
            pivot.CalculateData();

            // Speichere die Arbeitsmappe
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


