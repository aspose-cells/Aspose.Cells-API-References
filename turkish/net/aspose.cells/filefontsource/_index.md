---
title: "Sınıf FileFontSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FileFontSource sınıfı. Dosya sisteminde depolanan tek TrueType yazı tipi dosyasını temsil eder"
type: docs
url: /tr/net/aspose.cells/filefontsource/
---
## FileFontSource class

Dosya sisteminde depolanan tek TrueType yazı tipi dosyasını temsil eder.

```csharp
public class FileFontSource : FontSourceBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Yazı tipi dosyasının yolu. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Yazı tipi kaynağının türünü döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // TrueType yazı tipi dosyasının yolunu belirtin
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // FileFontSource örneği oluşturun
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Yazı tipi kaynağı türünü ve dosya yolunu gösterin
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Workbook nesnesi oluşturun
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bir hücre değerini ayarlayın
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Özel yazı tipini hücreye uygulayın
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


