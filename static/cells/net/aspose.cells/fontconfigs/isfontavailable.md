##FontConfigs.IsFontAvailable
FontConfigs method. Indicate whether the font is available
## FontConfigs.IsFontAvailable method
Indicate whether the font is available.
```csharp
public static bool IsFontAvailable(string fontName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | String | font name |
### Return Value
true if font is available, otherwise false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsMethodIsFontAvailableWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Test font names to check availability
string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };
try
{
foreach (string fontName in testFonts)
{
// Call the IsFontAvailable method with the font name
bool isAvailable = FontConfigs.IsFontAvailable(fontName);
// Display the result
Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");
// Write the result to worksheet
int row = worksheet.Cells.MaxDataRow + 1;
worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
worksheet.Cells[row, 1].PutValue(isAvailable);
}
Console.WriteLine("Method executed successfully with parameters (String)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
}
// Save the result
workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
