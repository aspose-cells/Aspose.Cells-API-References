##Worksheet.Scenarios
Worksheet property. Gets the collection of Scenario
## Worksheet.Scenarios property
Gets the collection of [`Scenario`](../../scenario/).
```csharp
public ScenarioCollection Scenarios { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyScenariosDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Initial Value");
worksheet.Cells["A2"].PutValue(100);
// Add scenarios
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex1 = scenarios.Add("Scenario1");
Scenario scenario1 = scenarios[scenarioIndex1];
scenario1.Comment = "First test scenario";
int scenarioIndex2 = scenarios.Add("Scenario2");
Scenario scenario2 = scenarios[scenarioIndex2];
scenario2.Comment = "Second test scenario";
// Save the workbook
workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
// Clear scenarios and save again
scenarios.Clear();
workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
}
}
}
```
### See Also
* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
