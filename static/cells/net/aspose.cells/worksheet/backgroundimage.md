##Worksheet.BackgroundImage
Worksheet property. Gets and sets worksheet background image
## Worksheet.BackgroundImage property
Gets and sets worksheet background image.
```csharp
public byte[] BackgroundImage { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyBackgroundImageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Path to the image file
string imagePath = "background.jpg";
// Read the image file into a byte array
byte[] imageData = File.ReadAllBytes(imagePath);
// Set the background image for the worksheet
worksheet.BackgroundImage = imageData;
// Save the workbook
workbook.Save("WorksheetWithBackground.xlsx");
Console.WriteLine("Worksheet background image set successfully.");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
