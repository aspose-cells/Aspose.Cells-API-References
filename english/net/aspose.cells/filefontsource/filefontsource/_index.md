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
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Create a FileFontSource instance
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Display the font source type and file path
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Create a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Set a cell value
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Apply the custom font to the cell
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
```

### See Also

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


