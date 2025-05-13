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
public void Worksheet_Property_Scenarios()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "ScenarioTest.xlsx");
    ScenarioCollection scenarios = workbook.Worksheets[0].Scenarios;
    Assert.AreEqual(scenarios.Count, 2);
    scenarios.Clear();
    Assert.AreEqual(scenarios.Count, 0);
    workbook.Save(Constants.destPath + "ScenarioClearTest.xlsx");
    workbook = new Workbook(Constants.destPath + "ScenarioClearTest.xlsx");
    scenarios = workbook.Worksheets[0].Scenarios;
    Assert.AreEqual(0, scenarios.Count);
}
```

### See Also

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


