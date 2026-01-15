---
title: Class LowCodeImageSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.LowCodeImageSaveOptions class. Options for saving image in low code way
type: docs
url: /net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Options for saving image in low code way.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | The options for rendering images. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../lowcodesaveoptions/outputstream/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../lowcodesaveoptions/outputfile/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Gets or sets the save format. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Provider of save options for saving generated images. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to the worksheet
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // Create an instance of LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Set basic properties
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Display current settings
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Modify some image options
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Create a simple save options provider
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Save the worksheet as an image
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### See Also

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


