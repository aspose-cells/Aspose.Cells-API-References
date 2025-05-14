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
// Called: Assert.AreEqual(1, scenarios.LastSelected);
private void ScenarioCollection_Property_LastSelected(ScenarioCollection scenarios)
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

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


