---
title: "SmartTagCollection.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagCollection özelliği. Hücre smart tag'lerinin satırını alır"
type: docs
url: /tr/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Hücre akıllı etiketlerinin satırını alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine (satır 0, sütun 0) bir akıllı etiket ekle
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // A1 hücresi için SmartTagCollection'ı al
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Bu smart tag'leri içeren hücrenin satırını göster
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Not: Row özelliği yalnızca okunabilir, bu yüzden ayarlanamaz
            // smartTags.Row = 5; // Bu bir derleme hatasına neden olur

            // Farklı bir satırı göstermek için B3 hücresine (satır 2, sütun 1) başka bir smart tag ekle
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


