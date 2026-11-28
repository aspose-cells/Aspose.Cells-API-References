---
title: "PivotTable.CalculateData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Pivot tablonun verilerini hücrelere hesaplar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

PivotTable verilerini hücrelere hesaplar.

```csharp
public void CalculateData()
```

### Açıklamalar

Bu yöntem yalnızca [`PivotCache`](../pivotcache/) içindeki önbelleğe alınmış verilerle hesaplama yapar. En son veri kaynağıyla hesaplama yapmak istiyorsanız, lütfen [`Refresh`](../../pivotcache/refresh/) yöntemini kullanın. Yalnızca pivot tablonun ayarı değiştirildiyse, `CalculateData` yeterlidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Pivot tablo oluştur - doğru parametrelerin sağlanmasıyla düzeltildi
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Pivot'a alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Tarih filtresi uygula
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Pivot verilerini hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Seçeneklerle pivot tabloyu hesaplar.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenek | PivotTableCalculateOption | Pivot tabloyu hesaplamak için seçenekler |

### Dönüş Değeri

Hesaplanmış tüm pivot tabloları döndürür. Eğer [`RefreshData`](../../pivottablecalculateoption/refreshdata/) true ise, aynı pivot önbelleğine dayanan tüm pivot tablolar birlikte hesaplanır.

### Açıklamalar

Eğer [`RefreshData`](../../pivottablecalculateoption/refreshdata/) true ise, bu yöntem veri kaynağından pivot önbelleğini yeniler, ardından aynı pivot önbelleğine dayanan tüm pivot tabloları hesaplar. Aksi takdirde, yalnızca pivot önbelleğindeki önbelleğe alınmış verilerle hesaplama yapılır.

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Hesaplama seçeneklerini ayarlayın
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Seçeneklerle hesapla
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


