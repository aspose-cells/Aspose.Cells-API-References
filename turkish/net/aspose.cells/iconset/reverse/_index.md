---
title: "IconSet.Reverse"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconSet özelliği. Bu simge setindeki simgelerin varsayılan sırasının tersine çevrilip çevrilmeyeceğini belirten bayrağı alır veya ayarlar. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Bu ikon setindeki ikonların varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı alın veya ayarlayın. Varsayılan değer false'tur.

```csharp
public bool Reverse { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Aralığı ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Simge seti koşullu biçimlendirmesi oluştur
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Simge setini yapılandır
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Reverse özelliğini göster
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Çalışma kitabını kaydedin
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


