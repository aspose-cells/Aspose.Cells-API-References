---
title: "PivotField.CurrentPageItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Yalnızca bu pivot alanı sayfa alanı için şu anda görüntülenen sayfa öğesini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Bu pivot alanı için şu anda görüntülenen sayfa öğesini alır veya ayarlar (yalnızca sayfa alanı).

```csharp
public short CurrentPageItem { get; set; }
```

### Açıklamalar

Tümünü Seç'i göstermek için sentinel değer olarak [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) kullanın. Bu önceden tanımlanmış bir işaretçidir ve geçerli bir öğe indeksi değildir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Verileri yenileyin
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Sayfa alanlarını al
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Mevcut sayfa öğelerini göster
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Mevcut sayfa öğesini değiştir
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


