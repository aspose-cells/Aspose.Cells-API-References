---
title: Worksheet.Scenarios
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the collection of Scenario
type: docs
url: /net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Gets the collection of [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### Examples

```csharp
// Called: ScenarioCollection scenarios = workbook.Worksheets[0].Scenarios;
[Test]
        public void Property_Scenarios()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ScenarioTest.xlsx");
            ScenarioCollection scenarios = workbook.Worksheets[0].Scenarios;
            CheckScenarios(scenarios);
            workbook.Save(Constants.destPath + "InputCellsTest.xlsx");
            workbook = new Workbook(Constants.destPath + "InputCellsTest.xlsx");
            scenarios = workbook.Worksheets[0].Scenarios;
            CheckScenarios(scenarios);
        }
```

### See Also

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


