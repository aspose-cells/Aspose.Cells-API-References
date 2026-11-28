---
title: "PivotFilter.Value2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter özelliği. Etiket pivot filtresinin string value2 değerini alır."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/value2/
---
## PivotFilter.Value2 property

Etiket pivot filtresinin string değer2'sini alır.

```csharp
public string Value2 { get; set; }
```

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "WidgetA";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["A3"].Value = "WidgetB";
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["A4"].Value = "WidgetA";
            worksheet.Cells["B4"].Value = 75;

            int pivotIndex = worksheet.PivotTables.Add("A6", "A1:B4", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.Value1 = "100";
            filter.Value2 = "200";
            filter.MeasureFldIndex = 0;

            workbook.Save("PivotFilterValue2Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


