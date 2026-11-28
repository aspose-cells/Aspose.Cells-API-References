---
title: "PivotField.IsAutoSort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını gösterir.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoSort { get; set; }
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
    public class PivotFieldPropertyIsAutoSortDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin.
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Blueberry";
            cells["B5"].Value = 15;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Satır alanı ekle ve otomatik sıralamayı ayarla
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsAutoSort = true;
            rowField.AutoSortField = 1; // Sort by Quantity (column B)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldIsAutoSortDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


