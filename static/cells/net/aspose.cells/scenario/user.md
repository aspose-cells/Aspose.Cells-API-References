##Scenario.User
Scenario property. Gets name of user who last changed the scenario
## Scenario.User property
Gets name of user who last changed the scenario.
```csharp
public string User { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyUserDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex = scenarios.Add("TestScenario");
Scenario scenario = scenarios[scenarioIndex];
// Demonstrate User property usage
Console.WriteLine("Scenario created by user: " + scenario.User);
workbook.Save("ScenarioUserDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
