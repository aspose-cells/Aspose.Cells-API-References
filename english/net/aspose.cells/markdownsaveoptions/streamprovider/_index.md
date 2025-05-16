---
title: MarkdownSaveOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Gets or sets the IStreamProvider for exporting objects
type: docs
url: /net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Gets or sets the IStreamProvider for exporting objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.CustomStreamProvider
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Custom initialization logic for the stream
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Custom cleanup logic for the stream
            options.Stream?.Close();
        }
    }

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Create MarkdownSaveOptions instance
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Display current LightCellsDataProvider value (null by default)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "custom provider"));
            
            // Save with the options
            workbook.Save("MarkdownWithCustomStream.md", saveOptions);
            
            // Demonstrate effect by checking if file was created
            if (File.Exists("MarkdownWithCustomStream.md"))
            {
                Console.WriteLine("File saved successfully");
            }
        }
    }
}
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


