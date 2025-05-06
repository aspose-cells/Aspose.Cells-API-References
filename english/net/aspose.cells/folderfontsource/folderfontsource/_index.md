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
            string folderPath = @&quot;C:\Fonts&quot;;
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Accessing properties
            Console.WriteLine(&quot;Folder Path: &quot; + folderFontSource.FolderPath);
            Console.WriteLine(&quot;Scan Subfolders: &quot; + folderFontSource.ScanSubFolders);
            Console.WriteLine(&quot;Font Source Type: &quot; + folderFontSource.Type);

            // Create a workbook and set the font sources
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Save the workbook
            workbook.Save(&quot;FolderFontSourceExample.xlsx&quot;);
            workbook.Save(&quot;FolderFontSourceExample.pdf&quot;);
            return;
        }
```

### See Also

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


