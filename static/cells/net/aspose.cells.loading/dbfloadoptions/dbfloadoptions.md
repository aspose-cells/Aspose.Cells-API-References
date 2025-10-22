##DbfLoadOptions.DbfLoadOptions
DbfLoadOptions constructor. The options
## DbfLoadOptions constructor
The options.
```csharp
public DbfLoadOptions()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Loading;
using System;
public class DbfLoadOptionsMethodCtorDemo
{
public static void Run()
{
try
{
// Create DbfLoadOptions instance using the #ctor method
DbfLoadOptions loadOptions = new DbfLoadOptions();
// Create workbook with DBF load options
Workbook workbook = new Workbook("sample.dbf", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some data from the loaded DBF file
Console.WriteLine("Data loaded from DBF file:");
Console.WriteLine(worksheet.Cells["A1"].StringValue);
// Save the workbook in Excel format
workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("File saved successfully with DBF data");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)
