##ScenarioCollection.LastSelected
ScenarioCollection property. Indicates which scenario was last selected by the user to be run/shown
## ScenarioCollection.LastSelected property
Indicates which scenario was last selected by the user to be run/shown.
```csharp
public int LastSelected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ScenarioCollectionPropertyLastSelectedDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add scenarios
ScenarioCollection scenarios = worksheet.Scenarios;
scenarios.Add("Scenario1");
scenarios.Add("Scenario2");
// Set active scenario and last selected index
scenarios.ActiveIndex = 1;
scenarios.LastSelected = 1;
// Verify and demonstrate LastSelected property
Console.WriteLine("Total scenarios: " + scenarios.Count);
Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);
// Modify last selected index
scenarios.LastSelected = 0;
Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
}
}
}
```
### See Also
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
