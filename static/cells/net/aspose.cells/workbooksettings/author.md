##WorkbookSettings.Author
WorkbookSettings property. Gets and sets the author of the file
## WorkbookSettings.Author property
Gets and sets the author of the file.
```csharp
public string Author { get; set; }
```
### Remarks
It''s not set, check [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/) first, then check the user of Environment.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyAuthorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set the author property
settings.Author = "John Doe";
// Add some sample data to demonstrate workbook functionality
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Sample Workbook");
sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
sheet.Cells["A3"].PutValue(DateTime.Now.ToString());
// Save the workbook
workbook.Save("AuthorDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
