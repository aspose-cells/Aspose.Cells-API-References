---
title: "PivotField.AutoSortField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Otomatik sıralanan alanın dizinini temsil eder. 1, PivotField kendisini, diğerleri ise veri alanlarının konumunu ifade eder."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Otomatik sıralanan alanın dizinini temsil eder. -1, PivotField kendisini, diğerleri ise veri alanlarının konumunu ifade eder.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.SortSetting.SortBy özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Otomatik sıralamayı yapılandırın
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Verileri hesapla ve yenile
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


