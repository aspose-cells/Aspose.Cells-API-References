---
title: FolderFontSource.ScanSubFolders
second_title: Aspose.Cells for .NET API Reference
description: FolderFontSource property. Determines whether or not to scan the subfolders
type: docs
url: /net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Determines whether or not to scan the subfolders.

```csharp
public bool ScanSubFolders { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
public static void Property_ScanSubFolders()
        {
            // Create an instance of FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Accessing properties
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Create a workbook and set the font sources
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Save the workbook
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
```

### See Also

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


