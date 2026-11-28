---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling property. Sayfa indeksini veya adını dosya yoluna her zaman ekleyip eklemeyeceği. Varsayılan değer false'tur; bu, yalnızca bir sayfa olduğunda sayfa indeksi veya adı ve ilgili önek dosya yoluna eklenmez."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

Sayfa indeksinin veya adının dosya yoluna her zaman eklenip eklenmeyeceği. Varsayılan değer false'tur, yani yalnızca bir sayfa olduğunda, sayfa indeksi (veya adı) ve ilgili önek dosya yoluna eklenmez.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Bir worksheet içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // LowCodeSaveOptionsProviderOfAssembling örneği oluştur
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // Yol ayarlarını yapılandır
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // İlk özellik değerini göster
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // BuildPathWithSheetAlways olmadan dosya yolunu göster
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // BuildPathWithSheetAlways'ı true olarak ayarla
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // BuildPathWithSheetAlways ile dosya yolunu göster (tek sayfa olsa bile)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // Çalışma kitabını kaydet (bölme davranışı gerçek senaryolarda sağlayıcının ayarlarını kullanır)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


