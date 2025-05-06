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
// Called: Console.WriteLine(&amp;quot;Scan Subfolders: &amp;quot; + folderFontSource.ScanSubFolders);
public static void Property_ScanSubFolders()
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


