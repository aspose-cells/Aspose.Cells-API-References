##Style.Custom
Style property. Represents the custom number format string of this style object. If the custom number format is not setFor example the number format is builtin  will be returned
## Style.Custom property
Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.
```csharp
public string Custom { get; set; }
```
### Remarks
The returned custom string is culture-independent.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyCustomDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create and apply custom date format
Style style = workbook.CreateStyle();
style.Custom = "d-mmm-yy";
cells["A1"].PutValue(new DateTime(2023, 10, 15));
cells["A1"].SetStyle(style);
// Display the formatted value
Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
// Save the workbook
workbook.Save("StylePropertyCustomDemo_out.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
