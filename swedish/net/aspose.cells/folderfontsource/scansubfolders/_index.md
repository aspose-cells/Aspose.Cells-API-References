---
title: "FolderFontSource.ScanSubFolders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FolderFontSource-egenskap. Avgör om underkatalogerna ska skannas eller inte"
type: docs
url: /sv/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Bestämmer om underkataloger ska genomsökas eller inte.

```csharp
public bool ScanSubFolders { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Skapa en folder font source med skanning av underkataloger aktiverad
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Visa egenskaper för teckensnittskälla
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Skapa en workbook och ange font-källan
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Demonstrera användning genom att ange lite text
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Spara arbetsboken
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


