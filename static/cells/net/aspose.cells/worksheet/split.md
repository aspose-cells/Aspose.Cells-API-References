##Worksheet.Split
Worksheet method. Splits window
## Worksheet.Split method
Splits window.
```csharp
public void Split()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodSplitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to demonstrate split
worksheet.Cells["A1"].PutValue("Header");
for (int i = 1; i <= 50; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
}
// Split the worksheet (no parameters needed)
worksheet.Split();
// Save the workbook
workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
