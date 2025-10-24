##Metered.IsMeteredLicensed
Metered method. Check whether metered is licensed
## Metered.IsMeteredLicensed method
Check whether metered is licensed
```csharp
public static bool IsMeteredLicensed()
```
### Return Value
True or false
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class MeteredMethodIsMeteredLicensedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a Metered instance
Metered metered = new Metered();
try
{
// Check if metered license is applied
bool isLicensed = Metered.IsMeteredLicensed();
// Display the result
Console.WriteLine($"Is Metered Licensed: {isLicensed}");
// Add the result to the worksheet
worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
worksheet.Cells["B1"].PutValue(isLicensed);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
}
// Save the result
workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
