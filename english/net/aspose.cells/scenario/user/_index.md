---
title: Scenario.User
second_title: Aspose.Cells for .NET API Reference
description: Scenario property. Gets name of user who last changed the scenario
type: docs
url: /net/aspose.cells/scenario/user/
---
## Scenario.User property

Gets name of user who last changed the scenario.

```csharp
public string User { get; }
```

### Examples

```csharp
// Called: string user = scenario.User;
public static void Scenario_Property_User()
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


