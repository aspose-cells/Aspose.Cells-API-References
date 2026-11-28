---
title: "Class FolderFontSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FolderFontSource sınıfı. TrueType yazı tipi dosyalarını içeren klasörü temsil eder."
type: docs
url: /tr/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

TrueType yazı tipi dosyalarını içeren klasörü temsil eder.

```csharp
public class FolderFontSource : FontSourceBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Yazı tipleri klasörünün yolu. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Alt klasörlerin taranıp taranmayacağını belirler. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Yazı tipi kaynağının türünü döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // FolderFontSource örneği oluştur
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Özelliklere erişim
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Bir workbook oluştur ve yazı tipi kaynaklarını ayarla
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Çalışma kitabını kaydedin
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


