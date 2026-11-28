---
title: "PivotField.FilterByValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Veri pivot alanının değerlerine göre filtreler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Veri pivot alanının değerlerine göre filtreler.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| valueFieldIndex | Int32 | Değer bölgesindeki değer alanının indeksi. |
| type | PivotFilterType | Filtreleme verisinin tipi. |
| value1 | Double | Filtre koşulunun değeri |
| value2 | Double | Aralık filtre koşulunun üst sınır değeri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
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
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanları ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // FilterByValue yöntemini (Int32, PivotFilterType, Double, Double) parametreleriyle çağırın
                // Miktar (alan indeksi 1) 90 ile 160 arasında olan ürünleri filtrele
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Değişiklikleri göstermek için pivot tabloyu yenileyin
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
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


