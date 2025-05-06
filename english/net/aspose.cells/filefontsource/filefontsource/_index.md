---
title: FileFontSource.FileFontSource
second_title: Aspose.Cells for .NET API Reference
description: FileFontSource constructor. Ctor
type: docs
url: /net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Ctor.

```csharp
public FileFontSource(string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | path to font file |

### Examples

```csharp
// Called: FileFontSource fontSource = new FileFontSource(fontFilePath);
public static void FileFontSource_Constructor()
        {
            // Specify the path to the TrueType font file
            string fontFilePath = &quot;C:\\Fonts\\CustomFont.ttf&quot;;

            // Create a FileFontSource instance
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Display the font source type and file path
            Console.WriteLine(&quot;Font Source Type: &quot; + fontSource.Type);
            Console.WriteLine(&quot;Font File Path: &quot; + fontSource.FilePath);

            // Create a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Set a cell value
            Cell cell = sheet.Cells[&quot;A1&quot;];
            cell.PutValue(&quot;Hello, Aspose!&quot;);

            // Apply the custom font to the cell
            Style style = cell.GetStyle();
            style.Font.Name = &quot;CustomFont&quot;; // Use the name of the font
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save(&quot;FileFontSourceExample.xlsx&quot;);
            workbook.Save(&quot;FileFontSourceExample.pdf&quot;);
        }
```

### See Also

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


