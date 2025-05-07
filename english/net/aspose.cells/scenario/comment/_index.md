---
title: Scenario.Comment
second_title: Aspose.Cells for .NET API Reference
description: Scenario property. Gets and sets the comment of scenario
type: docs
url: /net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Gets and sets the comment of scenario.

```csharp
public string Comment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("创建者 Simon 日期 6/19/2014", scenario.Comment);
private void Property_Comment(ScenarioCollection scenarios)
        {
            Assert.AreEqual(scenarios.Count, 2);
            Assert.AreEqual(1, scenarios.ActiveIndex);
            Assert.AreEqual(1, scenarios.LastSelected);
            Scenario scenario = scenarios[0];
            Assert.AreEqual("test", scenario.Name);
            Assert.AreEqual(true, scenario.IsLocked);
            Assert.AreEqual(false, scenario.IsHidden);
            Assert.AreEqual("Simon", scenario.User);
            Assert.AreEqual("创建者 Simon 日期 6/19/2014", scenario.Comment);
            Assert.AreEqual(scenario.InputCells.Count, 4);
            ScenarioInputCell inputCell = scenario.InputCells[0];
            Assert.AreEqual("G16", inputCell.Name);
            Assert.AreEqual("1", inputCell.Value);
        }
```

### See Also

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


