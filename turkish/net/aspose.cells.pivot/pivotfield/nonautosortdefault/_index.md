---
title: "PivotField.NonAutoSortDefault"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bu pivot alanına uygulanacak bir sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Bu pivot alanına uygulanacak bir sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen !PivotField.SortSetting.IsSimpleSort özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına ve pivot tabloya erişin
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Pivot tabloda ilk satır alanına erişin
            PivotField pivotField = pivotTable.RowFields[0];
            
            // NonAutoSortDefault özelliğini true olarak ayarlayın
            pivotField.NonAutoSortDefault = true;
            
            // Özellik değerini çıktı olarak ver
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


