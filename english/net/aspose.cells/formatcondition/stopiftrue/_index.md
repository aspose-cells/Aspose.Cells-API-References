---
title: FormatCondition.StopIfTrue
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. True no rules with lower priority may be applied over this rule when this rule evaluates to true. Only applies for Excel 2007
type: docs
url: /net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(fcs[0].StopIfTrue);
[Test]
        public void Property_StopIfTrue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CustomIconSet01.xlsx");
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.IsTrue(fcs[0].IconSet.IsCustom);
            Assert.IsFalse(fcs[0].StopIfTrue);
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


