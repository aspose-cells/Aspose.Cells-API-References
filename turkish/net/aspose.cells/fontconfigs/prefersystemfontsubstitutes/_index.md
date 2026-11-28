---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs özelliği. Bir yazı tipi sunulmadığında ve bu yazı tipinin ikamesi ayarlanmamışsa, sistem yazı tipi ikamelerini önce kullanıp kullanmayacağını belirtir. örn. Ubuntu'da Arial yazı tipi genellikle Liberation Sans ile ikame edilir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Bir yazı tipi mevcut olmadığında ve bu yazı tipinin ikamesi ayarlanmamış olduğunda sistem yazı tipi ikamelerini önce kullanıp kullanmayacağını belirtin. Örneğin Ubuntu'da "Arial" yazı tipi genellikle "Liberation Sans" ile ikame edilir. Varsayılan değer false'tur.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mevcut PreferSystemFontSubstitutes değerini göster
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // PreferSystemFontSubstitutes değerini true olarak ayarla
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // İkame gerekebilecek bir yazı tipine sahip bir hücre oluştur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Yazı tipi ikame etkilerini görmek için çalışma kitabını kaydet
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Varsayılan değere sıfırla
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


