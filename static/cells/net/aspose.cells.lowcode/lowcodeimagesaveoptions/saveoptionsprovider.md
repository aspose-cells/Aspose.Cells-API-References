##LowCodeImageSaveOptions.SaveOptionsProvider
LowCodeImageSaveOptions property. Provider of save options for saving generated images
## LowCodeImageSaveOptions.SaveOptionsProvider property
Provider of save options for saving generated images.
```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```
### Remarks
The output([`OutputFile`](../../lowcodesaveoptions/outputfile/) or [`OutputStream`](../../lowcodesaveoptions/outputstream/)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
using System;
public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Image Data");
// Create LowCodeImageSaveOptions instance
LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
saveOptions.SaveFormat = SaveFormat.Png;
saveOptions.ImageOptions = new ImageOrPrintOptions();
// Create a custom SaveOptionsProvider
CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
saveOptions.SaveOptionsProvider = provider;
// Display current SaveOptionsProvider
Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
// Demonstrate effect by saving with different options
workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
// Change to null provider
saveOptions.SaveOptionsProvider = null;
Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
}
}
public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
{
// Return custom save options for each part
return new LowCodeImageSaveOptions()
{
SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
ImageOptions = new ImageOrPrintOptions()
{
Quality = 90,
HorizontalResolution = 300,
VerticalResolution = 300
}
};
}
public override void Finish(LowCodeSaveOptions part)
{
// Perform any cleanup after saving
Console.WriteLine("Finished saving part with custom options");
}
}
}
```
### See Also
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
