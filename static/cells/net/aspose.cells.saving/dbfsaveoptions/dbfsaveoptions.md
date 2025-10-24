##DbfSaveOptions.DbfSaveOptions
DbfSaveOptions constructor. The options of saving .dbf file
## DbfSaveOptions constructor
The options of saving .dbf file.
```csharp
public DbfSaveOptions()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Saving;
using System;
public class DbfSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
try
{
// Create DbfSaveOptions instance using the constructor
DbfSaveOptions saveOptions = new DbfSaveOptions();
// Set properties of the save options
saveOptions.ExportAsString = true;
// Save the workbook with DBF save options
workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
}
catch (Exception ex)
{
Console.WriteLine($"Error saving DBF file: {ex.Message}");
}
}
}
}
```
### See Also
* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
