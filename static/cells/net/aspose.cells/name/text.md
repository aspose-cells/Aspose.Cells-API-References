##Name.Text
Name property. Gets the name text of the object
## Name.Text property
Gets the name text of the object.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a named range
int index = workbook.Worksheets.Names.Add("MyNamedRange");
Name namedRange = workbook.Worksheets.Names[index];
namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
// Set and display the Text property
namedRange.Text = "MyCustomName";
Console.WriteLine("Named range text: " + namedRange.Text);
// Save the workbook
workbook.Save("NamedRangeExample.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
