---
title: "FolderFontSource.ScanSubFolders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FolderFontSource özelliği. Alt klasörlerin taranıp taranmayacağını belirler"
type: docs
url: /tr/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Alt klasörlerin taranıp taranmayacağını belirler.

```csharp
public bool ScanSubFolders { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Alt klasör taraması etkinleştirilmiş bir klasör yazı tipi kaynağı oluşturun
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Yazı tipi kaynağı özelliklerini göster
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Bir çalışma kitabı oluşturun ve yazı tipi kaynağını ayarlayın
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Bazı metin ayarlayarak kullanımını gösterin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Çalışma kitabını kaydedin
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


