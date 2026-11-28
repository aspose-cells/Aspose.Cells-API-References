---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldSortSetting özelliği. Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir.

```csharp
public bool IsSimpleSort { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            // Sıralama ayarını al (yalnızca okunabilir özellik)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Mevcut IsSimpleSort değerini göster
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Not: IsSimpleSort yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Sıralamayı göstermek için, farklı bir sıralama ile yeni bir pivot tablo oluşturacağız

            // Özel sıralama ile başka bir pivot tablo oluştur
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot alanını mevcut yöntemi kullanarak sırala
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


