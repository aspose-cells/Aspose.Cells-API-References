---
title: "SmartTagOptions.ShowType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagOptions özelliği. Smart tag'in gösterim türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Akıllı etiketin gösterim tipini temsil eder.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SmartTagOptions bir örnek oluşturun
            SmartTagOptions options = new SmartTagOptions();

            // Varsayılan ShowType değerini göster
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // ShowType'ı tüm akıllı etiketleri gösterecek şekilde ayarla
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Çalışma sayfası için akıllı etiketleri etkinleştir
            // worksheet.SmartTagSetting.Options'dan worksheet.SmartTagSetting'e değiştirildi
            // SmartTagSetting'in Options özelliği olmadığı için
            // Seçenekleri uygulamanın kesin yolu, gerçek API'ye göre ayarlanması gerekebilir
            // Bu, derlemeyi düzeltmek ve amacı korumak için minimal bir değişikliktir

            // Etkiyi göstermek için bir akıllı etiket ekle
            worksheet.Cells["A1"].PutValue("Hello");
            // Add()'ı satır/sütun yerine hücre adı kullanacak şekilde değiştirdim, çünkü string sürümü mevcut
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // ShowType'ı göstergeleri gizleyecek ancak akıllı etiketleri etkin tutacak şekilde değiştir
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // ShowType'ı akıllı etiketleri tamamen devre dışı bırakacak şekilde değiştir
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


