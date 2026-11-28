---
title: "FolderFontSource.FolderPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FolderFontSource özelliği. Yazı tipleri klasörünün yolu"
type: docs
url: /tr/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Yazı tipleri klasörünün yolu.

```csharp
public string FolderPath { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Klasör yazı tipi kaynağı oluştur
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // FolderPath özelliğinin kullanımını gösterin
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Yazı tipi kaynağıyla bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Basit gösterim - özel yazı tipleri kullanabilecek metin ekleyin
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Çıktıları kaydedin
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


