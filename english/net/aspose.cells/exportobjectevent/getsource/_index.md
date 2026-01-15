---
title: ExportObjectEvent.GetSource
second_title: Aspose.Cells for .NET API Reference
description: ExportObjectEvent method. Gets the object to be exported
type: docs
url: /net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Gets the object to be exported.

```csharp
public object GetSource()
```

### Return Value

the object to be exported.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a picture to demonstrate the GetSource functionality
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Create a custom export object listener
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Save the workbook to trigger the ExportObjectEvent
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Demonstrate the GetSource method
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### See Also

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


