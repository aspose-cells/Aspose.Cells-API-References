##Hyperlink.TextToDisplay
Hyperlink property. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink
## Hyperlink.TextToDisplay property
Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.
```csharp
public string TextToDisplay { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkPropertyTextToDisplayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add hyperlinks with TextToDisplay property
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
// Add first hyperlink with custom display text
int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
// Add second hyperlink with custom display text
int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
hyperlinks[index2].TextToDisplay = "Aspose Documentation";
// Add third hyperlink with cell reference as display text
int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
// Save the workbook
string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
workbook.Save(outputPath, SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
}
}
}
```
### See Also
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
