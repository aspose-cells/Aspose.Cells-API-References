---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldSortSetting özelliği. Sıralanan alanın indeksini temsil eder. 1, PivotField'i etiketlere göre sıralamak anlamına gelir; diğerleri ise veri alanına göre sıralama anlamına gelir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Sıralanan alanın indeksini temsil eder. -1, PivotField'i etiketlere göre sıralamak anlamına gelir; diğerleri ise veri alanına göre sıralama anlamına gelir.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotFieldSortSetting.SortBy özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Pivot alanı sıralama ayarını al
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Mevcut FieldIndex değerini göster
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Not: FieldIndex yalnızca okunabilir ve PivotFieldSortSetting doğrudan örneklenemez
            // çünkü genel bir yapıcıya sahip değildir. Yalnızca mevcut örnekle çalışabiliriz
            // pivot alanının SortSetting özelliğinden elde edilir.

            // Değişiklikleri uygulamak için özet tabloyu yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Sonucu kaydet
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


