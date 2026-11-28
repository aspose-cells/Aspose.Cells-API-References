---
title: "PivotField.IsRepeatItemLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Alanın etiketlerinin satır veya sütun bölgesinde tekrarlanıp tekrarlanmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Alan etiketlerinin satır veya sütun bölgesinde tekrarlanıp tekrarlanmayacağını gösterir. Varsayılan değer yanlıştır.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");

            // Pivot tabloyu içeren çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];

            // İlk satır alanı için öğe etiketlerinin tekrarlanmasını etkinleştir
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // İlk sütun alanı için öğe etiketlerinin tekrarlanmasını etkinleştir
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


