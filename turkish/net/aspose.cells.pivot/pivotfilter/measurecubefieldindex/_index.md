---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter özelliği. Ölçü küp alanının dizinini belirtir. Bu özellik yalnızca OLAP pivotlarındaki filtreler tarafından kullanılır ve bir değer filtresinin hangi ölçüde uygulanacağını belirler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Ölçü küp alanının dizinini belirtir. Bu özellik yalnızca OLAP pivotlarındaki filtreler tarafından kullanılır ve bir değer filtresinin hangi ölçüye uygulanacağını belirtir.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve örnek veri ile doldur
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Bir pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır ve veri alanları ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Pivot tabloya bir filtre ekle
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // PivotField yerine PivotTable üzerinden filtre oluştur ve ekle
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // MeasureCubeFieldIndex'i göster
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


