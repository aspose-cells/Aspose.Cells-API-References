---
title: "PivotFieldCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldCollection yöntemi. PivotField nesnesini belirli tip PivotFields'e ekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Belirli PivotFields türüne bir PivotField nesnesi ekler.

```csharp
public int Add(PivotField pivotField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotField | PivotField | bir PivotField nesnesi. |

### Dönüş Değeri

Bu PivotFields içindeki PivotField nesnesinin indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            
            // Add yöntemi kullanarak veri alanını sütun alanları bölgesine ekle
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Pivot tablo verilerini hesapla
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


