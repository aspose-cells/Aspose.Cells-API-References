---
title: "Enum FontSourceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontSourceType enum. Bir yazı tipi kaynağının türünü belirtir"
type: docs
url: /tr/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Yazı tipi kaynağının türünü belirtir.

```csharp
public enum FontSourceType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| FontFile | `0` | tek bir yazı tipi dosyasını temsil eder. |
| FontsFolder | `1` | Yazı tipi dosyaları içeren bir klasörü temsil eder. |
| MemoryFont | `2` | Bellekte tek bir yazı tipini temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // FontSourceType enum değerlerini gösterin
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Yazı tipi ayarlarını oluşturun ve FontSourceType'ı kullanın
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Bir hücreye yazı tipini uygulayın
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Sonucu kaydet
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


