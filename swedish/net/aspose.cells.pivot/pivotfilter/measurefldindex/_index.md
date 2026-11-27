---
title: "PivotFilter.MeasureFldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter egenskap. Hämtar måttfältets index för pivotfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Hämtar måttfältets index för pivotfiltret.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotFilter.ValueFieldIndex egenskap. Denna metod kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

            // Hämta pivottabellsamlingen och lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta filterkollektionen och lägg till ett filter
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MeasureFldIndex = 1;

            workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


