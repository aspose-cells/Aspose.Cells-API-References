---
title: FormatCondition.Formula2
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets the value or expression associated with conditional formatting
type: docs
url: /net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Gets and sets the value or expression associated with conditional formatting.

```csharp
public string Formula2 { get; set; }
```

### Remarks

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".

### Examples

```csharp
// Called: Assert.AreEqual(condition1.Formula2, condition2.Formula2, "!" + sheetName + "--FormatCondition.getFormula2");
private static void Property_Formula2(
            String sheetName,
            ConditionalFormattingCollection cfc1,
            ConditionalFormattingCollection cfc2)
        {
            for (int i = 0; i < cfc1.Count; i++)
            {
                FormatConditionCollection fcc1 = cfc1[i];
                FormatConditionCollection fcc2 = cfc2[i];
                for (int conditionIndex = 0; conditionIndex < fcc1.Count; conditionIndex++)
                {
                    FormatCondition condition1 = fcc1[conditionIndex];
                    FormatCondition condition2 = fcc2[conditionIndex];
                    Assert.AreEqual(condition1.Formula2, condition2.Formula2, "!" + sheetName + "--FormatCondition.getFormula2");
                    Assert.AreEqual(condition1.Formula1, condition2.Formula1, "!" + sheetName + "--FormatCondition.getFormula1");
                }
            }
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


