---
title: "PivotTable.IsAutoFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. Excel 2003 için pivottable seçeneğinde bulunan otomatik biçimlendirme kutucuğu."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

**PivotTable** raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. Excel 2003'teki pivottable seçeneğinde bulunan "autoformat table" onay kutusu

```csharp
public bool IsAutoFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsAutoFormatDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // IsAutoFormat özelliğini ayarla
            pivotTable.IsAutoFormat = true; // Enable auto formatting
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


