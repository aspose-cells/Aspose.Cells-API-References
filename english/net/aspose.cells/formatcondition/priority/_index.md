---
title: FormatCondition.Priority
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values where 1 is the highest priority
type: docs
url: /net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

```csharp
public int Priority { get; set; }
```

### Examples

```csharp
// Called: var priority1 = rule1[0].Priority;
[Test]
        public void Property_Priority()
        {
            var workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CellsNet47425.xlsx");

            var rule1 = workbook.Worksheets["Sheet1"].ConditionalFormattings[0];
            var priority1 = rule1[0].Priority;
            Assert.AreEqual(4, priority1);
            Assert.IsTrue(workbook.Worksheets.Dxfs.Count == 0);
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


