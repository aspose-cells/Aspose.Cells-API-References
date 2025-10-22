##Class Scenario
Aspose.Cells.Scenario class. Represents an individual scenario
## Scenario class
Represents an individual scenario.
```csharp
public class Scenario
```
## Properties
| Name | Description |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Gets and sets the comment of scenario. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Gets the input cells of scenario. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Indicates whether scenario is hidden. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Indicates whether scenario is locked for editing when the sheet is protected. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Gets and sets the name of scenario. |
| [User](../../aspose.cells/scenario/user/) { get; } | Gets name of user who last changed the scenario. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ScenarioDemo
{
public static void ScenarioExample()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the scenario collection of the worksheet
ScenarioCollection scenarios = worksheet.Scenarios;
// Add a new scenario to the collection
int scenarioIndex = scenarios.Add("MyScenario");
Scenario scenario = scenarios[scenarioIndex];
// Setting properties of the scenario
scenario.Comment = "This is a test scenario.";
scenario.Name = "TestScenario";
scenario.IsHidden = false;
scenario.IsLocked = true;
// Accessing read-only properties
string user = scenario.User;
ScenarioInputCellCollection inputCells = scenario.InputCells;
// Save the workbook
workbook.Save("ScenarioExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
