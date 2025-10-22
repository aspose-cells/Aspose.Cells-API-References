##Worksheet.Name
Worksheet property. Gets or sets the name of the worksheet
## Worksheet.Name property
Gets or sets the name of the worksheet.
```csharp
public string Name { get; set; }
```
### Remarks
The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and set its name
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "DataSheet";
// Add a new worksheet with a specific name
Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
// Output the names of all worksheets
Console.WriteLine("Worksheet Names:");
foreach (Worksheet ws in workbook.Worksheets)
{
Console.WriteLine(ws.Name);
}
// Save the workbook
workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
