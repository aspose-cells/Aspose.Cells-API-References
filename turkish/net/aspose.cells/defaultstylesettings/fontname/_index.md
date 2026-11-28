---
title: "DefaultStyleSettings.FontName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DefaultStyleSettings özelliği. Çalışma kitabı için varsayılan yazı tipi adını alır/ayarlar"
type: docs
url: /tr/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Çalışma kitabı için varsayılan yazı tipi adını alır/ayarlar

```csharp
public string FontName { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Yükleme seçenekleri oluştur ve yazı tipi adını ayarla
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Yükleme seçenekleriyle yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Varsayılan stile eriş ve yazı tipi adını doğrula
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Bir çalışma sayfası oluştur ve hücre değerini ayarla
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Çalışma kitabını kaydedin
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


