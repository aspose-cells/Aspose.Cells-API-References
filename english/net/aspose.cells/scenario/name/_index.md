---
title: Scenario.Name
second_title: Aspose.Cells for .NET API Reference
description: Scenario property. Gets and sets the name of scenario
type: docs
url: /net/aspose.cells/scenario/name/
---
## Scenario.Name property

Gets and sets the name of scenario.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: scenario.Name = &amp;quot;TestScenario&amp;quot;;
public static void Property_Name()
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

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


