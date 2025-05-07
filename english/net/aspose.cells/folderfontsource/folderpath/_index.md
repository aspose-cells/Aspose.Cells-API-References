---
title: FolderFontSource.FolderPath
second_title: Aspose.Cells for .NET API Reference
description: FolderFontSource property. Path to fonts folder
type: docs
url: /net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Path to fonts folder.

```csharp
public string FolderPath { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
public static void Property_FolderPath()
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


