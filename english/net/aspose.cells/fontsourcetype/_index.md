---
title: Enum FontSourceType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontSourceType enum. Specifies the type of a font source
type: docs
url: /net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Specifies the type of a font source.

```csharp
public enum FontSourceType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| FontFile | `0` | represents a single font file. |
| FontsFolder | `1` | Represents a folder with font files. |
| MemoryFont | `2` | Represents a single font in memory. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrate FontSourceType enum values
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Create font settings and use FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Apply font to a cell
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Save the result
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


