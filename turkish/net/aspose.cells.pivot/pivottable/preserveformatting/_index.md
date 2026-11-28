---
title: "PivotTable.PreserveFormatting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesi PivotTableFormat'ın korunup korunmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesi ([`PivotTableFormat`](../../pivottableformat/)) korunup korunmadığını gösterir.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotTable.PreserveCellFormattingOnUpdate özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("source.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Yenileme sırasında biçimlendirmeyi korumayı etkinleştir
            pivotTable.PreserveFormatting = true;
            
            // Pivot tablo veri alanına bazı biçimlendirmeler uygulayın
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Pivot tablo veri alanını biçimlendirin
            pivotTable.FormatAll(style);
            
            // Pivot tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


