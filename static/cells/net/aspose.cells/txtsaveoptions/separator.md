##TxtSaveOptions.Separator
TxtSaveOptions property. Gets and sets char Delimiter of text file
## TxtSaveOptions.Separator property
Gets and sets char Delimiter of text file.
```csharp
public char Separator { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertySeparatorDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Configure TXT save options with comma separator
TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
txtSaveOptions.Separator = ',';
txtSaveOptions.Encoding = System.Text.Encoding.UTF8;
// Save the workbook as CSV with comma separator
string outputPath = "output.csv";
workbook.Save(outputPath, txtSaveOptions);
// Display the saved file content
Console.WriteLine("File saved with comma separator:");
Console.WriteLine(File.ReadAllText(outputPath));
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
