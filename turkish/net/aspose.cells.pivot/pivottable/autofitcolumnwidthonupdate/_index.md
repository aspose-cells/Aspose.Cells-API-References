---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Güncelleme sırasında sütun genişliğinin otomatik ayarlanıp ayarlanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Güncelleme sırasında sütun genişliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir.

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // Pivot tabloyu içeren çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Güncelleme sırasında sütun genişliğinin otomatik ayarlanmasını devre dışı bırak
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Değişiklikleri uygulamak için pivot tabloyu yenile
            worksheet.RefreshPivotTables();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


