---
title: "PivotFilter.EvaluationOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Eigenschaft. Gibt die Auswertungsreihenfolge des Pivot-Filters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

Ermittelt die Auswertungsreihenfolge des Pivotfilters.

```csharp
public int EvaluationOrder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten befüllen
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // Felder hinzufügen
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot-Filter hinzufügen
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // Setzen Sie Filtereigenschaften einschließlich EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Pivot-Tabelle aktualisieren
            pivot.RefreshData();
            pivot.CalculateData();

            // Arbeitsmappe speichern.
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


