---
title: "PivotTable.ShowEmptyCol"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Boş sütunların tabloya dahil edilip edilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir.

```csharp
public bool ShowEmptyCol { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // ShowEmptyCol değerinin mevcut durumunu göster
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // ShowEmptyCol değerini false olarak ayarla (boş sütunları gizle)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // Pivot tablo verilerini hesapla
            pivotTable.CalculateData();

            // Boş sütunlar gizli olarak çalışma kitabını kaydet
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // ShowEmptyCol değerini true olarak ayarla (boş sütunları göster)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // Pivot tablo verilerini tekrar hesapla
            pivotTable.CalculateData();

            // Boş sütunlar görünür olarak çalışma kitabını kaydet
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


