##ImageConverter.Process
ImageConverter method. Converts template file to images
## Process(string, string) {#process_2}
Converts template file to images.
```csharp
public static void Process(string templateFile, string resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted to images. |
| resultFile | String | The resultant file(name pattern) for generated images. |
### Remarks
The output files will be build from the specified result file by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class ImageConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
// Create a new workbook and populate with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));
// Save as template file for processing
workbook.Save("Template.xlsx", SaveFormat.Xlsx);
try
{
// Convert template to images using (String, String) parameters
ImageConverter.Process("Template.xlsx", "OutputSheet.png");
Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during image conversion: {ex.Message}");
}
}
}
}
```
### See Also
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts template file to images
```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
### Remarks
When converting to image of format that supports multiple pages(such as tiff), the specified [`OutputFile`](../../lowcodesaveoptions/outputfile/) or [`OutputStream`](../../lowcodesaveoptions/outputstream/) will be used directly for the resultant image.  For other types of image, if the save options has specified Stream as output, then all resultant images will be saved to the same Stream. Otherwise, the output files will be build from the specified output file of the save options by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.LowCode;
using System;
public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
try
{
// Initialize LowCodeLoadOptions with a template file
LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
// Initialize LowCodeSaveOptions with output directory
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
// Execute Process method with specified parameters
ImageConverter.Process(loadOptions, saveOptions);
Console.WriteLine("Spreadsheet converted to images successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during processing: {ex.Message}");
}
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}
Converts template file to images
```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions,
AbstractLowCodeSaveOptionsProvider provider)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for saving. Its output([`OutputFile`](../../lowcodesaveoptions/outputfile/) or [`OutputStream`](../../lowcodesaveoptions/outputstream/)) takes no effect because all outputs will be specified by the "provider" parameter |
| provider | AbstractLowCodeSaveOptionsProvider | Provider of save options for saving the generated images |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
{
public static void Run()
{
const string templatePath = "SampleTemplate.xlsx";
const string outputDir = "Output/";
// Create sample template
CreateTemplateFile(templatePath);
Directory.CreateDirectory(outputDir);
// Initialize load options
var loadOptions = new LowCodeLoadOptions()
{
InputFile = templatePath // Fixed property name
};
// Configure save options using LowCodeImageSaveOptions
var saveOptions = new LowCodeImageSaveOptions() // Corrected class
{
SaveFormat = SaveFormat.Png // Corrected property and enum
};
var provider = new DynamicSaveOptionsProvider(saveOptions);
try
{
// Call static Process method
ImageConverter.Process(loadOptions, saveOptions, provider);
Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
}
catch (Exception ex)
{
Console.WriteLine($"Processing failed: {ex.Message}");
}
}
private static void CreateTemplateFile(string path)
{
using (Workbook wb = new Workbook())
{
Worksheet sheet = wb.Worksheets[0];
sheet.Cells["A1"].PutValue("LowCode Process Demo");
sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
wb.Save(path, SaveFormat.Xlsx);
}
}
private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type
public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
{
_baseOptions = options;
}
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
{
// Access resolution properties from LowCodeImageSaveOptions
if (partInfo.SheetIndex == 0)
{
_baseOptions.ImageOptions.HorizontalResolution = 300;
_baseOptions.ImageOptions.VerticalResolution = 300;
}
return _baseOptions;
}
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
