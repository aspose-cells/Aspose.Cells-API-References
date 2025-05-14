---
title: Scenario.IsLocked
second_title: Aspose.Cells for .NET API Reference
description: Scenario property. Indicates whether scenario is locked for editing when the sheet is protected
type: docs
url: /net/aspose.cells/scenario/islocked/
---
## Scenario.IsLocked property

Indicates whether scenario is locked for editing when the sheet is protected.

```csharp
public bool IsLocked { get; set; }
```

### Examples

```csharp
// Called: scenario.IsLocked = true;
public static void Scenario_Property_IsLocked()
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
```

### See Also

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


