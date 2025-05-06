---
title: ScenarioCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ScenarioCollection method. Adds a scenario
type: docs
url: /net/aspose.cells/scenariocollection/add/
---
## ScenarioCollection.Add method

Adds a scenario.

```csharp
public int Add(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of scenario. |

### Return Value

The index in the list of scenarios.

### Examples

```csharp
// Called: int scenarioIndex = scenarios.Add(&amp;quot;MyScenario&amp;quot;);
public static void Method_String_()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the scenario collection of the worksheet
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Add a new scenario to the collection
            int scenarioIndex = scenarios.Add(&quot;MyScenario&quot;);
            Scenario scenario = scenarios[scenarioIndex];

            // Setting properties of the scenario
            scenario.Comment = &quot;This is a test scenario.&quot;;
            scenario.Name = &quot;TestScenario&quot;;
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Accessing read-only properties
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Save the workbook
            workbook.Save(&quot;ScenarioExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


