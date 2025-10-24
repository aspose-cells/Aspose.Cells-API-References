##JsonSaveOptions.SheetIndexes
JsonSaveOptions property. Represents the indexes of exported sheets
## JsonSaveOptions.SheetIndexes property
Represents the indexes of exported sheets.
```csharp
public int[] SheetIndexes { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class JsonSaveOptionsPropertySheetIndexesDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Populate some data in each sheet
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Worksheet sheet = workbook.Worksheets[i];
sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
}
// Create JsonSaveOptions instance
JsonSaveOptions options = new JsonSaveOptions();
// Display current SheetIndexes (null by default - exports all sheets)
Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));
// Set to export only first and third sheets (indexes 0 and 2)
options.SheetIndexes = new int[] { 0, 2 };
// Save to JSON with selected sheets
workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);
// Verify by loading the JSON
string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
Console.WriteLine("JSON Content:");
Console.WriteLine(jsonContent);
// Change to export only the second sheet (index 1)
options.SheetIndexes = new int[] { 1 };
workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);
// Verify the single sheet export
jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
Console.WriteLine("Single Sheet JSON Content:");
Console.WriteLine(jsonContent);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
