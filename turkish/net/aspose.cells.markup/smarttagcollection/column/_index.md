---
title: "SmartTagCollection.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagCollection özelliği. Hücre smart tag'lerinin sütununu alır"
type: docs
url: /tr/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Hücre akıllı etiketlerinin sütununu alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // C5 hücresine (satır 4, sütun 2) bir smart tag ekle
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // C5 hücresi için SmartTagCollection'ı al
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Bu smart tag'leri içeren hücrenin sütununu göster
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Farklı bir sütunu göstermek için E2 hücresine (satır 1, sütun 4) başka bir smart tag ekle
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


