---
title: "Sınıf FontSourceBase"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontSourceBase sınıfı. Kullanıcının çeşitli yazı tipi kaynaklarını belirtmesine izin veren sınıflar için soyut bir temel sınıftır"
type: docs
url: /tr/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Bu, kullanıcının çeşitli yazı tipi kaynaklarını belirtmesine izin veren sınıflar için soyut bir temel sınıftır

```csharp
public abstract class FontSourceBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Yazı tipi kaynağının türünü döndürür. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Klasör yazı tipi kaynağı oluştur
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Yazı tipi kaynağı özelliklerini göster
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Çalışma kitabı oluştur ve yazı tipi kaynağını ayarla
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Özel yazı tipleriyle kaydet
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


