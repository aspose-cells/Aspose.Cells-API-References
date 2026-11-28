---
title: "Class DefaultStyleSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DefaultStyleSettings sınıfı. Çalışma kitaplarının stil özelliklerinin varsayılan değerleri için ayarlar"
type: docs
url: /tr/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Çalışma kitabının stil özelliklerinin varsayılan değerleri için ayarlar.

```csharp
public class DefaultStyleSettings
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Stil hem yerleşik sayı hem de özel desen tanımladığında sayı biçimi özelliğinin tercih edilip edilmediğini gösterir. Varsayılan değer false'tur, bu da varsayılan olarak bir stil için özel desen boş olmadığı sürece değerleri biçimlendirmek için kullanılacağı anlamına gelir. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Çalışma kitabı için varsayılan yazı tipi adını alır/ayarlar |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Çalışma kitabı için varsayılan standart yazı tipi boyutunu alır/ayarlar. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Yatay hizalama için varsayılan değeri alır/ayarlar |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Dikey hizalama için varsayılan değeri alır/ayarlar |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabının varsayılan stil ayarlarına erişin
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Özellikleri ayarlama
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Varsayılan stil ayarlarını ilk çalışma sayfasına uygulayın
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Çalışma kitabını kaydedin
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


