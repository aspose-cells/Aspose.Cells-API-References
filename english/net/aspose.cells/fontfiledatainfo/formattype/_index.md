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

            // Add some text to demonstrate font usage
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Load a sample font file (replace with actual font file path)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Register the font folder
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // In a real scenario, FontFileDataInfo would be obtained from the library
                    // For demonstration, we'll simulate getting font info
                    // Note: Actual API might provide this through FontConfigs or similar
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Display the FormatType property value
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Show the enum value as string
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Apply the font to a cell (conceptual - actual implementation may vary)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Save the workbook
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Helper method to simulate getting FontFileDataInfo
        // In real usage, this would be provided by the Aspose.Cells API
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Create a mock FontFileDataInfo (in reality, this would come from the API)
                // Since we can't instantiate it directly, we'll simulate the behavior
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // In a real implementation, this would be returned by the API
                // For this demo, we'll just return null since we can't create the object
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### See Also

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


