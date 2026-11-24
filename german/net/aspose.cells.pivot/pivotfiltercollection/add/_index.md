---
title: "PivotFilterCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilterCollection-Methode. Fügt ein PivotFilter-Objekt dem angegebenen Typ hinzu"
type: docs
url: /de/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Fügt ein PivotFilter-Objekt dem angegebenen Typ hinzu

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | der PivotField-Index |
| Typ | PivotFilterType | der PivotFilter-Typ |

### Rückgabewert

der Index des PivotFilter-Objekts in dieser PivotFilterCollection.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methoden PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() und AddDateFilter(). Diese Methode wird 12 Monate nach November 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionMethodAddWithInt32PivotFilterTypeDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten
            cells["A1"].Value = "Category";
            cells["A2"].Value = "A";
            cells["A3"].Value = "B";
            cells["A4"].Value = "A";
            cells["A5"].Value = "B";
            
            cells["B1"].Value = "Value";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;
            cells["B5"].Value = 40;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // Pivot-Filter hinzufügen
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            pivot.RefreshData();
            pivot.CalculateData();

            book.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


