##ScenarioCollection.ActiveIndex
ScenarioCollection property. Gets and sets which scenario is selected
## ScenarioCollection.ActiveIndex property
Gets and sets which scenario is selected.
```csharp
public int ActiveIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioCollectionPropertyActiveIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ScenarioCollection scenarios = worksheet.Scenarios;
int scenarioIndex = scenarios.Add("TestScenario");
scenarios.ActiveIndex = scenarioIndex;
Console.WriteLine($"Active scenario index set to: {scenarios.ActiveIndex}");
workbook.Save("ScenarioActiveIndexDemo.xlsx");
}
}
}
```
### See Also
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
