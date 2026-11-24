---
title: "PivotFilter.MeasureFldIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Eigenschaft. Gibt den Index des Messfelds des Pivotfilters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Gibt den Index des Messfelds des Pivotfilters zurück.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PivotFilter.ValueFieldIndex. Diese Methode wird 12 Monate später, seit November 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureFldIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 400;

            // Abrufen der Pivot‑Tabellensammlung und Hinzufügen einer Pivot‑Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Abrufen der Filter‑Sammlung und Hinzufügen eines Filters
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MeasureFldIndex = 1;

            workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


