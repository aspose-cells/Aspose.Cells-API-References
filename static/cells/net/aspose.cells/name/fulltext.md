##Name.FullText
Name property. Gets the name full text of the object with the scope setting
## Name.FullText property
Gets the name full text of the object with the scope setting.
```csharp
public string FullText { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyFullTextDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create some named ranges
worksheet.Cells["A1"].PutValue("Test Value");
worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
// Get the names collection
NameCollection names = workbook.Worksheets.Names;
// Find a name by its FullText
string reference = "=Sheet1!$A$1:$B$5";
Name foundName = FindNameByFullText(names, reference);
// Output results
if (foundName != null)
{
Console.WriteLine("Found name: " + foundName.Text);
Console.WriteLine("FullText: " + foundName.FullText);
}
else
{
Console.WriteLine("Name not found");
}
}
public static Name FindNameByFullText(NameCollection names, string reference)
{
if (reference.IndexOf('=') == 0)
{
reference = reference.Substring(1);
}
foreach (Name nm in names)
{
if (nm.FullText.Equals(reference))
{
return nm;
}
}
return null;
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
