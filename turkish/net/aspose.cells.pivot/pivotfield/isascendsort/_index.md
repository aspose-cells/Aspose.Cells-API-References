---
title: "PivotField.IsAscendSort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bu pivot alanının öğelerinin artan şekilde otomatik sıralanıp sıralanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Bu pivot alanının öğelerinin artan şekilde otomatik olarak sıralanıp sıralanmadığını gösterir.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendSort { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen **PivotField.SortSetting.SortType** özelliğini veya **PivotField.SortBy()** yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendSortDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "B";
            sheet.Cells["A3"].Value = "C";
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B2"].Value = 150;
            sheet.Cells["B3"].Value = 300;
            sheet.Cells["B4"].Value = 200;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Sıralamayı yapılandır
            PivotField sortField = pivotTable.RowFields[0];
            sortField.IsAutoSort = true;
            sortField.IsAscendSort = false; // Demonstrate descending sort
            sortField.AutoSortField = 0; // Sort by first data field
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldIsAscendSortDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


