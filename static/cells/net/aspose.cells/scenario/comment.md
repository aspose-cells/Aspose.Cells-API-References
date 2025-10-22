##Scenario.Comment
Scenario property. Gets and sets the comment of scenario
## Scenario.Comment property
Gets and sets the comment of scenario.
```csharp
public string Comment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a scenario collection
ScenarioCollection scenarios = worksheet.Scenarios;
// Add a scenario
int index = scenarios.Add("test");
Scenario scenario = scenarios[index];
// Set scenario properties
scenario.IsLocked = true;
scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
// Add input cells to the scenario using cell references and values
scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
scenario.InputCells.Add(0, 0, "100"); // A1
scenario.InputCells.Add(1, 1, "200"); // B2
scenario.InputCells.Add(2, 2, "300"); // C3
// Display scenario comment
Console.WriteLine("Scenario Comment: " + scenario.Comment);
// Save the workbook
workbook.Save("ScenarioCommentDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
