---
title: ScenarioCollection.ActiveIndex
second_title: Aspose.Cells for .NET API Reference
description: ScenarioCollection property. Gets and sets which scenario is selected
type: docs
url: /net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Gets and sets which scenario is selected.

```csharp
public int ActiveIndex { get; set; }
```

### Examples

```csharp
// Called: scenarios.ActiveIndex = scenarioIndex;
public static void Property_ActiveIndex()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ScenarioCollection of the worksheet
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Add a new scenario to the collection
            int scenarioIndex = scenarios.Add("Scenario1");

            // Access the newly added scenario
            Scenario scenario = scenarios[scenarioIndex];

            // Set some properties for the scenario
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // Set the active scenario index
            scenarios.ActiveIndex = scenarioIndex;

            // Set the last selected scenario index
            scenarios.LastSelected = scenarioIndex;

            // Save the workbook
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


