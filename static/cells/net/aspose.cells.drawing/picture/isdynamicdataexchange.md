##Picture.IsDynamicDataExchange
Picture property. Gets or sets whether dynamic data exchange
## Picture.IsDynamicDataExchange property
Gets or sets whether dynamic data exchange
```csharp
public bool IsDynamicDataExchange { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyIsDynamicDataExchangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Demonstrate IsDynamicDataExchange property
Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
// Set IsDynamicDataExchange to true
picture.IsDynamicDataExchange = true;
Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);
// Save the workbook
workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
