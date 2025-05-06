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
// Called: Assert.AreEqual(&amp;quot;Simon&amp;quot;, scenario.User);
private void Property_User(ScenarioCollection scenarios)
        {
            Assert.AreEqual(scenarios.Count, 2);
            Assert.AreEqual(1, scenarios.ActiveIndex);
            Assert.AreEqual(1, scenarios.LastSelected);
            Scenario scenario = scenarios[0];
            Assert.AreEqual(&quot;test&quot;, scenario.Name);
            Assert.AreEqual(true, scenario.IsLocked);
            Assert.AreEqual(false, scenario.IsHidden);
            Assert.AreEqual(&quot;Simon&quot;, scenario.User);
            Assert.AreEqual(&quot;创建者 Simon 日期 6/19/2014&quot;, scenario.Comment);
            Assert.AreEqual(scenario.InputCells.Count, 4);
            ScenarioInputCell inputCell = scenario.InputCells[0];
            Assert.AreEqual(&quot;G16&quot;, inputCell.Name);
            Assert.AreEqual(&quot;1&quot;, inputCell.Value);
        }
```

### See Also

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


