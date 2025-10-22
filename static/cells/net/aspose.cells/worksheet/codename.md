##Worksheet.CodeName
Worksheet property. Gets worksheet code name
## Worksheet.CodeName property
Gets worksheet code name.
```csharp
public string CodeName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCodeNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display the default CodeName
Console.WriteLine("Default CodeName: " + worksheet.CodeName);
// Change the CodeName
worksheet.CodeName = "MySheet";
Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
// Add a new worksheet and show its CodeName
Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
// Save the workbook
workbook.Save("WorksheetCodeNameDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
