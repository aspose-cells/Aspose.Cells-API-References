##Font.Equals
Font method. Checks if two fonts are equals
## Font.Equals method
Checks if two fonts are equals.
```csharp
public bool Equals(Font font)
```
| Parameter | Type | Description |
| --- | --- | --- |
| font | Font | Compared font object. |
### Return Value
True if equal to the compared font object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontMethodEqualsWithFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two font objects to compare
Font font1 = workbook.CreateStyle().Font;
font1.Name = "Arial";
font1.Size = 12;
font1.IsBold = true;
font1.Color = System.Drawing.Color.Black;
Font font2 = workbook.CreateStyle().Font;
font2.Name = "Arial";
font2.Size = 12;
font2.IsBold = true;
font2.Color = System.Drawing.Color.Black;
try
{
// Call the Equals method to compare the fonts
bool areEqual = font1.Equals(font2);
// Display the result
Console.WriteLine($"The fonts are equal: {areEqual}");
// Modify one font to make them different
font2.IsItalic = true;
areEqual = font1.Equals(font2);
Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("FontEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
