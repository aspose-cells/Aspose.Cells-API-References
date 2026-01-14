---
title: HtmlSaveOptions.EmbeddedFontType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the type of embedding font file into html file. Default value is None which indicates that no font will be embedded in html
type: docs
url: /net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Gets or sets the type of embedding font file into html file. Default value is None which indicates that no font will be embedded in html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Create HTML save options
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Display the default EmbeddedFontType value
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Set EmbeddedFontType to Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Save the workbook with WOFF font embedding
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Reset to None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Save the workbook without font embedding
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


