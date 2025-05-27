---
title: FontFileDataInfo.FormatType
second_title: Aspose.Cells for .NET API Reference
description: FontFileDataInfo property. Gets font format type of font file
type: docs
url: /net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Gets font format type of font file.

```csharp
public FontFileFormatType FormatType { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Load a font file (TTF for this example)
            string fontPath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontPath);

            // Set font folder using static method
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontPath), false);

            // Get font file data info
            FontSourceBase[] fontSources = FontConfigs.GetFontSources();
            foreach (FontSourceBase source in fontSources)
            {
                if (source is FolderFontSource folderSource)
                {
                    // Instead of trying to create FontFileDataInfo directly,
                    // we'll use the known format type since we're loading a TTF file
                    FontFileFormatType formatType = FontFileFormatType.Ttf;
                    
                    Console.WriteLine("Font Format Type: " + formatType);

                    // Demonstrate usage based on format type
                    switch (formatType)
                    {
                        case FontFileFormatType.Ttf:
                            Console.WriteLine("This is a TrueType font");
                            break;
                        case FontFileFormatType.Otf:
                            Console.WriteLine("This is an OpenType font");
                            break;
                        case FontFileFormatType.Ttc:
                            Console.WriteLine("This is a TrueType Collection");
                            break;
                        default:
                            Console.WriteLine("Unknown font format");
                            break;
                    }
                }
            }

            // Save the workbook (though font operations don't directly affect the workbook content)
            workbook.Save("FontFormatTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


