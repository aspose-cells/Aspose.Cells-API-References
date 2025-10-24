##JsonLoadOptions.MultipleWorksheets
JsonLoadOptions property. Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes
## JsonLoadOptions.MultipleWorksheets property
Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes.
```csharp
public bool MultipleWorksheets { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
{
public static void Run()
{
// Create JSON load options with MultipleWorksheets enabled
JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
// Load JSON file into workbook with the specified options
Workbook workbook = new Workbook("example.json", options);
// Access data from the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Display some sample values from the loaded JSON
Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
}
}
}
```
### See Also
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
