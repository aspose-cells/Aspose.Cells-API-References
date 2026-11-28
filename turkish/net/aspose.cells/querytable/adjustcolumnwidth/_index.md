---
title: "QueryTable.AdjustColumnWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTable özelliği. Nesnenin AdjustColumnWidth değerini döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı sütun genişliklerine sahip örnek veri ekle
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Sütun genişliklerini manuel olarak ayarla
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Bir sorgu tablosu oluştur (gerçek oluşturma dış veri kaynağı gerektirdiği için simüle edilmiştir)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Mevcut AdjustColumnWidth değerini göster
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // AdjustColumnWidth değerini true olarak ayarla ve etkisini göster
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Sorgu tablosunu yenilemeyi simüle et (normalde sütun genişliklerini ayarlardı)
            // Gerçek bir senaryoda, bu sorgu tablosu verilerini yenilediğinde olur
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // AdjustColumnWidth değerini false olarak ayarla ve etkisini göster
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Yenilemeyi tekrar simüle et (artık orijinal sütun genişliklerini korur)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Çalışma kitabını kaydedin
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


