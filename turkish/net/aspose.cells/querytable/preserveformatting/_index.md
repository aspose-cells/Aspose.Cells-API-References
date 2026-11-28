---
title: "QueryTable.PreserveFormatting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTable özelliği. Nesnenin PreserveFormatting değerini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar.

```csharp
public bool PreserveFormatting { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve biçimlendirme ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Veri aralığına biçimlendirme uygula
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Aralıktaki her hücreye stil uygula
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Bir sorgu tablosu oluştur (gerçek oluşturma dış veri kaynağı gerektirdiği için simüle edilmiştir)
            // Gerçek kullanımda, bunu dış bir bağlantıdan oluşturursunuz
            QueryTable queryTable = worksheet.QueryTables[0];

            // Mevcut PreserveFormatting değerini göster
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // PreserveFormatting'i false olarak ayarla (yenileme sırasında mevcut biçimlendirmeyi korumaz)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Sorgu tablosunu yenilemeyi simüle et (PreserveFormatting false olduğunda genellikle biçimlendirmeyi temizler)
            // Gerçek bir senaryoda, bu sorgu tablosu verilerini yenilediğinde olur
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // PreserveFormatting'i tekrar true olarak ayarla
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Yenilemeyi tekrar simüle et (artık biçimlendirmeyi korur)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Çalışma kitabını kaydedin
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


