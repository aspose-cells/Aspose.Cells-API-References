---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Kullanışsız şekillerin göz ardı edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Gereksiz şekillerin yok sayılıp sayılmayacağını gösterir.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Açıklamalar

Yalnızca xlsx, xlsb ve xlsm dosyalarında çalışır. Bazı dosyalarda işe yaramayan, birbirinin üstüne binen aynı şekiller vardır; dosyaları yüklerken bunları göz ardı edebiliriz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Yükleme seçeneklerini oluştur ve IgnoreUselessShapes'i true olarak ayarla
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook("example.xlsx", options);

            // İlk çalışma sayfasındaki şekil sayısını çıktı olarak ver
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


