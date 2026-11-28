---
title: "Range.CurrentRegion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Geçerli bölgeyi temsil eden bir Range nesnesi döndürür. Geçerli bölge, boş satır ve boş sütunların herhangi bir kombinasyonu ile sınırlanan bir aralıktır."
type: docs
url: /tr/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

Mevcut bölgeyi temsil eden bir Range nesnesi döndürür. Mevcut bölge, boş satır ve boş sütunların herhangi bir kombinasyonu ile sınırlanan bir aralıktır.

```csharp
public Range CurrentRegion { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bölgeler oluşturmak için bazı boş hücrelerle verileri doldurun
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Bölgeleri ayırmak için 5. satırı boş bırakın
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // İlk bölgedeki bir hücreyi alın ve Range'e dönüştürün
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // İkinci bölgedeki bir hücreyi alın ve Range'e dönüştürün
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // Tüm geçerli bölgeye biçimlendirme uygulayın
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


