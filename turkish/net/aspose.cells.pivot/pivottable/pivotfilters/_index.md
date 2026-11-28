---
title: "PivotTable.PivotFilters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Pivot tablo içindeki tüm filtreleri döndürür"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Pivot tablo içindeki tüm filtreleri döndürür.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Bir pivot tablo oluştur
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Pivot tabloya alanlar ekle
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // PivotFilters koleksiyonuna erişin (yalnızca okunabilir özellik)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // PivotFilters koleksiyonu hakkında bilgileri göster
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Filtreler üzerinde yineleme yap ve türlerini göster
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // İşlevselliği göstermek için örnek bir filtre ekle
                if (pivotFilters.Count == 0)
                {
                    // İlk alana (Satış) bir değer filtresi ekle
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Güncellenmiş filtre sayısını göster
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Çalışma kitabını kaydedin
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


