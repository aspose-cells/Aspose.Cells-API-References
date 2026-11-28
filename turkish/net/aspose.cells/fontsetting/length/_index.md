---
title: "FontSetting.Length"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSetting özelliği. Karakterlerin uzunluğunu alır"
type: docs
url: /tr/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Karakterlerin uzunluğunu alır.

```csharp
public int Length { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine biraz metin ekleyin
            worksheet.Cells["A1"].PutValue("Hello World");

            // A1 hücresindeki metin için yazı tipi ayarları oluştur
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Length özelliğinin kullanımını göster
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Yazı tipi ayarının uzunluğunu değiştir
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Yazı tipi ayarına biçimlendirme uygula
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


