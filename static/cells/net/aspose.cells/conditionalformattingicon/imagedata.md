##ConditionalFormattingIcon.ImageData
ConditionalFormattingIcon property. Gets the icon set data
## ConditionalFormattingIcon.ImageData property
Gets the icon set data.
```csharp
public byte[] ImageData { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingIconPropertyImageDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and conditional formatting
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Get conditional formatting result
var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
if (conditionalFormattingResult != null)
{
ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
if (icon != null)
{
// Get the icon image data
byte[] imageData = icon.ImageData;
// Verify and display image information
if (imageData != null && imageData.Length > 0)
{
Console.WriteLine($"Icon data length: {imageData.Length} bytes");
}
}
}
}
}
}
```
### See Also
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
