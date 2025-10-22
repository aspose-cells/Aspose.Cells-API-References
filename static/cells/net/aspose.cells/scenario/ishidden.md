##Scenario.IsHidden
Scenario property. Indicates whether scenario is hidden
## Scenario.IsHidden property
Indicates whether scenario is hidden.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyIsHiddenDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ScenarioCollection scenarios = worksheet.Scenarios;
int index = scenarios.Add("TestScenario");
Scenario scenario = scenarios[index];
// Demonstrate IsHidden property
scenario.IsHidden = true;
Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
scenario.IsHidden = false;
Console.WriteLine("Scenario hidden status: " + scenario.IsHidden);
workbook.Save("ScenarioIsHiddenDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
