---
title: "FolderFontSource.FolderPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FolderFontSource-egenskap. Sökväg till teckensnittsmappen"
type: docs
url: /sv/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Sökväg till teckensnittsmappen.

```csharp
public string FolderPath { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Skapa en teckensnittskälla i en mapp
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Demonstrera användning av FolderPath-egenskapen
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Skapa arbetsbok med teckensnittskällan
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Enkel demonstration - lägg till text som kan använda anpassade teckensnitt
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Spara utdata
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


