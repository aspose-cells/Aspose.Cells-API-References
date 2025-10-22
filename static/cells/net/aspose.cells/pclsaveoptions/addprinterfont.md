##PclSaveOptions.AddPrinterFont
PclSaveOptions method. Adds information about font that is already added to the printer by manufacturer
## PclSaveOptions.AddPrinterFont method
Adds information about font that is already added to the printer by manufacturer.
```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontFullName | String | Full name of the font (e.g. "Times New Roman Bold Italic") used in the source file. |
| fontPclName | String | Name of the font that will be used in the output Pcl document. |
### Remarks
There are 52 fonts that are to be built in any printer according to Pcl specification. However manufactures can add some other fonts to their devices.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some text to the worksheet to demonstrate font usage
worksheet.Cells["A1"].PutValue("This text will use the added printer font");
// Create PCL save options
PclSaveOptions pclSaveOptions = new PclSaveOptions();
try
{
// Call the AddPrinterFont method with specific font names
pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
// Save the workbook with PCL options
workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
