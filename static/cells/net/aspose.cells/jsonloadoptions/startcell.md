##JsonLoadOptions.StartCell
JsonLoadOptions property. Gets and sets the start cell
## JsonLoadOptions.StartCell property
Gets and sets the start cell.
```csharp
public string StartCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonLoadOptionsPropertyStartCellDemo
{
public static void Run()
{
// Create JSON load options with StartCell property
JsonLoadOptions options = new JsonLoadOptions
{
StartCell = "B3" // JSON data will start from cell B3
};
// Create a workbook from JSON file with options
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("Header");
// Create a sample JSON file
System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
// Load JSON data into workbook
workbook = new Workbook("data.json", options);
// Save the workbook
workbook.Save("JsonStartCellDemo.xlsx");
}
}
}
```
### See Also
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
