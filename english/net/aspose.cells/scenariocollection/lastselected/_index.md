---
title: ScenarioCollection.LastSelected
second_title: Aspose.Cells for .NET API Reference
description: ScenarioCollection property. Indicates which scenario was last selected by the user to be run/shown
type: docs
url: /net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Indicates which scenario was last selected by the user to be run/shown.

```csharp
public int LastSelected { get; set; }
```

### Examples

```csharp
// Called: scenarios.LastSelected = scenarioIndex;
public static void Property_LastSelected()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the ScenarioCollection of the worksheet
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Add a new scenario to the collection
            int scenarioIndex = scenarios.Add(&quot;Scenario1&quot;);

            // Access the newly added scenario
            Scenario scenario = scenarios[scenarioIndex];

            // Set some properties for the scenario
            scenario.Comment = &quot;This is a test scenario.&quot;;
            scenario.IsHidden = false;

            // Set the active scenario index
            scenarios.ActiveIndex = scenarioIndex;

            // Set the last selected scenario index
            scenarios.LastSelected = scenarioIndex;

            // Save the workbook
            workbook.Save(&quot;ScenarioCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


