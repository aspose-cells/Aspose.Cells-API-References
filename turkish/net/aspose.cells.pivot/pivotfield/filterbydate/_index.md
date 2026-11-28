---
title: "PivotField.FilterByDate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Satır veya sütun pivot alanının tarih değerlerine göre filtreler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Satır veya sütun pivot alanının tarih değerlerine göre filtreler.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | PivotFilterType | Filtreleme verisinin tipi. |
| dateTime1 | DateTime | Filtre koşulunun tarih etiketi |
| dateTime2 | DateTime | Aralık filtre koşulunun üst sınır tarih etiketi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Tarihlerle örnek veri ekle
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Tarih alanını sütun bölgesine ekleyin
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Tarih filtresini uygula (2020-2021 arasındaki Eylül tarihleri)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Sonuçları kaydedin
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


