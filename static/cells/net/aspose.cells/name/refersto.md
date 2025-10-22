##Name.RefersTo
Name property. Returns or sets the formula that the name is defined to refer to beginning with an equal sign
## Name.RefersTo property
Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.
```csharp
public string RefersTo { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyRefersToDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "Sheet1";
// Add named ranges with RefersTo
int index1 = workbook.Worksheets.Names.Add("NamedRange1");
workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
int index2 = workbook.Worksheets.Names.Add("NamedRange2");
workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";
// Display RefersTo property of named ranges
Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
