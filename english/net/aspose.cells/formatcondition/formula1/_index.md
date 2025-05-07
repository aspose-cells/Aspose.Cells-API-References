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
// Called: string fml = fc.Formula1;
[Test]
        public void Property_Formula1()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/ConditionalFormatTest_002.xls");
            ConditionalFormattingCollection cfs = workbook.Worksheets[0].ConditionalFormattings;
            FormatCondition fc = cfs[0][0];
            string fml = fc.Formula1;
            if (!string.IsNullOrEmpty(fml) && fml[0] != '=')
            {
                fml = "=" + fml;
            }
            Assert.AreEqual("=1", fml);
            fml = fc.Formula2;
            if (!string.IsNullOrEmpty(fml) && fml[0] != '=')
            {
                fml = "=" + fml;
            }
            Assert.AreEqual("=2", fml);
            Assert.AreEqual(fc.Operator, OperatorType.Between);
            Assert.AreEqual(fc.Type, FormatConditionType.CellValue);
            fc = cfs[1][0];
            Assert.AreEqual(fc.Formula1, "=B2=3");
            Assert.AreEqual(fc.Type, FormatConditionType.Expression);
            workbook.Save(Constants.destPath + "ConditionalFormatTest_002.xls");
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


