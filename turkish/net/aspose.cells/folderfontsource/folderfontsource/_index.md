---
title: "FolderFontSource.FolderFontSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FolderFontSource yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Yapıcı.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| folderPath | String | yazı tipleri klasörünün yolu |
| scanSubfolders | Boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourceMethodCtorWithStringBooleanDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


