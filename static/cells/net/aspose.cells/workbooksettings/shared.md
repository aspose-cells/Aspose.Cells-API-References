##WorkbookSettings.Shared
WorkbookSettings property. Gets or sets a value that indicates whether the Workbook is shared
## WorkbookSettings.Shared property
Gets or sets a value that indicates whether the Workbook is shared.
```csharp
public bool Shared { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertySharedDemo
{
public static void Run()
{
// Create a new workbook
Workbook book = new Workbook();
// Set the Shared property to true
book.Settings.Shared = true;
// Save the workbook
string outputPath = "output_shared.xlsx";
book.Save(outputPath);
// Load the saved workbook to verify the Shared property
Workbook loadedBook = new Workbook(outputPath);
Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
