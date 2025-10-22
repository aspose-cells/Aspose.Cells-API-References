##PclSaveOptions.PclSaveOptions
PclSaveOptions constructor. Creates the options for saving pdf file
## PclSaveOptions constructor
Creates the options for saving pdf file.
```csharp
public PclSaveOptions()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PclSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
try
{
// Call the #ctor method to create PclSaveOptions instance
PclSaveOptions pclOptions = new PclSaveOptions();
// Configure additional options if needed
pclOptions.AddPrinterFont("Arial", "ArialPCL");
Console.WriteLine("PclSaveOptions created successfully");
// Save the workbook with PCL options
workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
}
catch (Exception ex)
{
Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
}
}
}
}
```
### See Also
* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
