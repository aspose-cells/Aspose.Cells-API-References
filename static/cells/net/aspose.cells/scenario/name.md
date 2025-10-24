##Scenario.Name
Scenario property. Gets and sets the name of scenario
## Scenario.Name property
Gets and sets the name of scenario.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex = scenarios.Add("InitialScenario");
Scenario scenario = scenarios[scenarioIndex];
// Demonstrate Name property usage
Console.WriteLine("Original scenario name: " + scenario.Name);
scenario.Name = "RenamedScenario";
Console.WriteLine("Updated scenario name: " + scenario.Name);
workbook.Save("ScenarioNameDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
