##IFilePathProvider.GetFullName
IFilePathProvider method. Gets the full path of the file by Worksheet name when exporting Worksheet to html separately. So the references among the Worksheets can be exported correctly
## IFilePathProvider.GetFullName method
Gets the full path of the file by Worksheet name when exporting Worksheet to html separately. So the references among the Worksheets can be exported correctly.
```csharp
public string GetFullName(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |
### Return Value
the full path of the file
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IFilePathProviderMethodGetFullNameWithStringDemo
{
public static void Run()
{
// Create a custom implementation of IFilePathProvider
CustomFilePathProvider provider = new CustomFilePathProvider();
// Call the GetFullName method with a sheet name
string sheetName = "Sheet1";
string fullPath = provider.GetFullName(sheetName);
// Display the result
Console.WriteLine($"Full path for {sheetName}: {fullPath}");
}
}
internal class CustomFilePathProvider : IFilePathProvider
{
public string GetFullName(string sheetName)
{
// Simple implementation that returns a path combining the sheet name with a directory
return $"C:\\Temp\\{sheetName}.xlsx";
}
}
}
```
### See Also
* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
