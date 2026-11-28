---
title: "FontConfigs.DefaultFontName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs özelliği. Varsayılan yazı tipi adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Varsayılan yazı tipi adını alır veya ayarlar.

```csharp
public static string DefaultFontName { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mevcut varsayılan yazı tipi adını göster
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Yeni bir varsayılan yazı tipi adı ayarla
            FontConfigs.DefaultFontName = "Arial";

            // Varsayılan yazı tipi kullanımını göstermek için açık bir yazı tipi ayarlanmamış bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Yazı tipinin doğru uygulandığını doğrula
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


