---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Anger indexet för måttkubfältet. Denna egenskap används endast av filter i OLAP-pivoter och anger på vilket mått ett värdefilter ska tillämpas"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Anger indexet för måttkubfältet. Denna egenskap används endast av filter i OLAP-pivoter och specificerar på vilket mått ett värdefilter ska tillämpas.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureCubeFieldIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Lägg till ett filter i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // Skapa och lägg till filter via PivotTable istället för PivotField
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // Visa MeasureCubeFieldIndex
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // Spara arbetsboken
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


