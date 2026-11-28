---
title: "PivotField.GetSubtotals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Bu pivot alanı için belirtilen alt toplamı gösterip göstermeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Bu pivot alanı için belirtilen alt toplamın gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Alt toplam türü. |

### Dönüş Değeri

Belirtilen alt toplamın gösterilip gösterilmediğini döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Toplam alt toplamının etkin olup olmadığını kontrol et
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Ortalama alt toplamının etkin olup olmadığını kontrol et
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Toplam alt toplamını etkinleştir
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Toplam alt toplamının şimdi etkin olduğunu doğrula
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Değişiklikleri göstermek için pivot tabloyu yenileyin
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


