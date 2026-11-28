---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Yapıcı.

```csharp
public IndividualFontConfigs()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // IndividualFontConfigs ile yükleme seçenekleri oluşturun
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Varsayılan çalışma sayfası ile yeni bir çalışma kitabı oluşturun
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Bir çalışma sayfasına erişin ve bazı metinler ekleyin
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Çalışma kitabını kaydet (kaydetme için yükleme seçeneklerine gerek yok)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


