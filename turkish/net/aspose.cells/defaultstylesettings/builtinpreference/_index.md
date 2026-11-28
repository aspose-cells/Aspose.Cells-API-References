---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DefaultStyleSettings özelliği. Stil hem yerleşik sayı hem de özel desen tanımladığında sayı biçimi özelliğinin tercih edilip edilmediğini gösterir. Varsayılan değer false'tur; bu, varsayılan olarak özel desenin, bir stil için boş olmadığı sürece değerleri biçimlendirmek için kullanılacağı anlamına gelir."
type: docs
url: /tr/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Stil hem yerleşik sayı hem de özel desen tanımladığında sayı biçimi özelliğinin tercih edilip edilmediğini gösterir. Varsayılan değer false'tur, bu da varsayılan olarak bir stil için özel desen boş olmadığı sürece değerleri biçimlendirmek için kullanılacağı anlamına gelir.

```csharp
public bool BuiltInPreference { get; set; }
```

### Açıklamalar

Mevcut şablon dosyasından çalışma kitabı yüklenirken, bir stil için hem yerleşik sayı hem de özel desen tanımlanmış olabilir. Bu özellik, stil ile değerleri biçimlendirirken yerleşik sayıyı mı yoksa özel deseni mi kullanmamız gerektiğini belirler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Varsayılan stil ayarlarına eriş
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // BuiltInPreference özelliğini göster
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Çalışma sayfasına uygula
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Çalışma kitabını kaydedin
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


