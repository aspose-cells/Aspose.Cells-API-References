##Worksheet.TabId
Worksheet property. Specifies the internal identifier for the sheet
## Worksheet.TabId property
Specifies the internal identifier for the sheet.
```csharp
public int TabId { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTabIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the TabId property
worksheet.TabId = 107;
// Save the workbook
string outputPath = "output.xlsb";
workbook.Save(outputPath);
// Load the saved workbook to verify the TabId
Workbook loadedWorkbook = new Workbook(outputPath);
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Display the TabId value
Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
