---
title: ScenarioInputCell.Name
second_title: Aspose.Cells for .NET API Reference
description: ScenarioInputCell property. Gets and sets the input cell address
type: docs
url: /net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Gets and sets the input cell address.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("G16", inputCell.Name);
private void Property_Name(ScenarioCollection scenarios)
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

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


