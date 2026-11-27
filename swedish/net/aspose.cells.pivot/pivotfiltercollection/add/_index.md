---
title: "PivotFilterCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection‑metod. Lägger till ett PivotFilter Object till den specifika typen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Lägger till ett PivotFilter Object till den specifika typen

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | PivotField‑indexet |
| typ | PivotFilterType | PivotFilter‑typen |

### Returvärde

Indexet för PivotFilter Object i denna PivotFilterCollection.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() och AddDateFilter() metoder. Denna metod kommer att tas bort 12 månader senare sedan november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

            // Exempeldata
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

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // Lägg till pivotfilter
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

### Se även

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


