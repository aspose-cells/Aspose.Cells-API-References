---
title: FolderFontSource.FolderFontSource
second_title: Aspose.Cells for .NET API Reference
description: FolderFontSource constructor. Ctor
type: docs
url: /net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Ctor.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| folderPath | String | path to fonts folder |
| scanSubfolders | Boolean | Determines whether or not to scan subfolders. |

### Examples

```csharp
// Called: FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);
public static void FolderFontSource_Constructor()
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


