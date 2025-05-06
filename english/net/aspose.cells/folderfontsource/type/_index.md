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
// Called: Console.WriteLine(&amp;quot;Font Source Type: &amp;quot; + folderFontSource.Type);
public static void Property_Type()
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

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


