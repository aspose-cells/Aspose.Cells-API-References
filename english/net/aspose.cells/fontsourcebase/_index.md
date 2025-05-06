---
title: Class FontSourceBase
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontSourceBase class. This is an abstract base class for the classes that allow the user to specify various font sources
type: docs
url: /net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

This is an abstract base class for the classes that allow the user to specify various font sources

```csharp
public abstract class FontSourceBase
```

## Properties

| Name | Description |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Returns the type of the font source. |

### Examples

```csharp
// Called: FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
public static void Type_FontSourceBase()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


