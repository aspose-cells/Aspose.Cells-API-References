---
title: "Enum FilterCategory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FilterCategory enum. Filtre kategorisini temsil eder"
type: docs
url: /tr/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Filtre kategorisini temsil eder.

```csharp
public enum FilterCategory
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Filtre Yok. |
| Label | `1` | Başlık Filtresi. |
| NumberValue | `2` | Sayısal Değer Filtresi. |
| Date | `3` | Tarih Değer Filtresi. |
| Top10 | `4` | Top10 Değer Filtresi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            CreateSampleData(worksheet);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanlarını yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Veri alanını yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Etiket filtresini özet filtrelerine ekle
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // FilterCategory kullanımını göster
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Özet tabloda tüm filtre kategorilerini göster
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Sonucu kaydet
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Örnek veri başlıklarını ayarla
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Örnek veri satırları ekle
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


