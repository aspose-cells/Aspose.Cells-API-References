##Scenario.IsLocked
Scenario property. Indicates whether scenario is locked for editing when the sheet is protected
## Scenario.IsLocked property
Indicates whether scenario is locked for editing when the sheet is protected.
```csharp
public bool IsLocked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioPropertyIsLockedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex = scenarios.Add("LockedScenario");
Scenario scenario = scenarios[scenarioIndex];
scenario.IsLocked = true;
Console.WriteLine("Scenario locked status: " + scenario.IsLocked);
workbook.Save("ScenarioLockDemo.xlsx");
}
}
}
```
### See Also
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
