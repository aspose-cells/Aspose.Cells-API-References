---
title: FormatCondition.Formula1
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets the value or expression associated with conditional formatting
type: docs
url: /net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Gets and sets the value or expression associated with conditional formatting.

```csharp
public string Formula1 { get; set; }
```

### Remarks

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".

### Examples

```csharp
// Called: Assert.AreEqual(cfs[0][0].Formula1, "=$E$1<=100");
[Test, Category("Bug")]
        public void FormatCondition_Property_Formula1()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Aspose_TEST_Merge.xml");
            ConditionalFormattingCollection cfs = workbook.Worksheets[0].ConditionalFormattings;
            Assert.AreEqual(cfs[0][0].Formula1, "=$E$1<=100");
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


