##ExternalLink.AddExternalName
ExternalLink method. Adds an external name
## ExternalLink.AddExternalName method
Adds an external name.
```csharp
public void AddExternalName(string text, string referTo)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the external name. If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | String | The referTo of the external name. It must be a cell or the range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkMethodAddExternalNameWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a sample external workbook
Workbook externalWorkbook = new Workbook();
Worksheet externalSheet = externalWorkbook.Worksheets[0];
externalSheet.Cells["B2"].PutValue(67);
// Add external link to the main workbook
string[] sheetNames = new string[] { externalSheet.Name };
int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
// Add external name
externalLink.AddExternalName("Test", "=Sheet1!$B$2");
// Use the external name in a formula
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
// Calculate the formula
workbook.CalculateFormula();
// Output the result
Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
