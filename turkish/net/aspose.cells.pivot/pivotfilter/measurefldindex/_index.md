---
title: "PivotFilter.MeasureFldIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter özelliği. Pivot filtresinin ölçü alanı indeksini alır."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Pivot filtresinin ölçü alanı indeksini alır.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotFilter.ValueFieldIndex özelliğini kullanın. Bu yöntem, Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

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

            // Pivot tablo koleksiyonunu al ve pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Filtre koleksiyonunu al ve filtre ekle
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MeasureFldIndex = 1;

            workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


