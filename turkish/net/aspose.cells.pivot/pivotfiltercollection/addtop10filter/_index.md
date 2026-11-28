---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilterCollection yöntemi. Veri pivot alanının değerlerine göre filtreler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

Veri pivot alanının değerlerine göre filtreler.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | Int32 | Kaynakta alanın dizini. |
| valueFieldIndex | Int32 | Veri bölgesindeki veri alanının indeksi. |
| type | PivotFilterType | Veri filtreleme türü. Sadece Sayım, Toplam ve Yüzde olabilir. |
| isTop | Boolean | Filtrenin üstten mi yoksa alttan mı uygulanacağını gösterir |
| itemCount | Int32 | Öğe sayısı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Pivot filtre koleksiyonunu al
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Top10 filtresi ekle - satışa göre en üst 2 öğeyi göster
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


