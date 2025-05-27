---
title: FolderFontSource.Type
second_title: Aspose.Cells for .NET API Reference
description: FolderFontSource property. Returns the type of the font source
type: docs
url: /net/aspose.cells/folderfontsource/type/
---
## FolderFontSource.Type property

Returns the type of the font source.

```csharp
public override FontSourceType Type { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### See Also

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


