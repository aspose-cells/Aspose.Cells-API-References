##LowCodeSplitOptions.SaveOptions
LowCodeSplitOptions property. Save options for saving the split parts
## LowCodeSplitOptions.SaveOptions property
Save options for saving the split parts.
```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSplitOptionsPropertySaveOptionsDemo
{
public static void Run()
{
// Create a new workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Create an instance of LowCodeSplitOptions
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
// Display initial SaveOptions value (null by default)
Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));
// Create and configure LowCodeSaveOptions for PDF format
LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
pdfSaveOptions.SaveFormat = SaveFormat.Pdf;
// Assign the save options to the SplitOptions
splitOptions.SaveOptions = pdfSaveOptions;
// Display updated SaveOptions value
Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);
// Example usage scenario: Splitting the workbook would save parts as PDF
// (Actual splitting code would depend on Aspose.Cells.LowCode API implementation)
// LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
// Save the original workbook for demonstration (not affected by SplitOptions)
workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
