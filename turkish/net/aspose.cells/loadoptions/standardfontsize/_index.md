---
title: "LoadOptions.StandardFontSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Varsayılan standart yazı tipi boyutunu ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Varsayılan standart yazı tipi boyutunu ayarlar.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Açıklamalar

NOTE: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluşturun ve StandardFontSize'i ayarlayın
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // İlk çalışma sayfasına ve hücrelere erişin.
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Bazı örnek metinler ayarlayın ve yazı tipi özelliklerini doğrulayın
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


