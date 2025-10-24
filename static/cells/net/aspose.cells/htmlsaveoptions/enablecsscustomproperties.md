##HtmlSaveOptions.EnableCssCustomProperties
HtmlSaveOptions property. Optimize the output of html by using CSS custom properties. For example for the scenario that there are multiple occurences for one base64 image with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false
## HtmlSaveOptions.EnableCssCustomProperties property
Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved. The default value is false.
```csharp
public bool EnableCssCustomProperties { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with formatting
worksheet.Cells["A1"].PutValue("Sample Text");
worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
// Add an image that will be repeated in multiple cells
int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
Picture pic = worksheet.Pictures[imgIndex];
pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
pic.Width = 100;
pic.Height = 100;
// Copy the image to another location
worksheet.Cells["D5"].PutValue("Same image reference:");
int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
Picture pic2 = worksheet.Pictures[imgIndex2];
pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
pic2.Width = 100;
pic2.Height = 100;
// Create HtmlSaveOptions instance
HtmlSaveOptions htmlOptions = new HtmlSaveOptions();
// Display current value
Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);
// Set to true to optimize CSS output
htmlOptions.EnableCssCustomProperties = true;
// Save with CSS optimization
workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);
// Set to false for comparison
htmlOptions.EnableCssCustomProperties = false;
workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);
Console.WriteLine("Files saved with and without CSS custom properties optimization.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
