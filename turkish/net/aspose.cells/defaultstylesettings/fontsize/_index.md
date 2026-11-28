---
title: "DefaultStyleSettings.FontSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DefaultStyleSettings özelliği. Çalışma kitabı için varsayılan standart yazı tipi boyutunu alır/ayarlar"
type: docs
url: /tr/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Çalışma kitabı için varsayılan standart yazı tipi boyutunu alır/ayarlar.

```csharp
public double FontSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Varsayılan yazı tipi adını ve boyutunu ayarla
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Bu ayarlarla HTML dosyasını yükle
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Bir hücreye erişin ve yazı tipinin boyutunu görüntüleyin
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Ayrıca Bakınız

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


