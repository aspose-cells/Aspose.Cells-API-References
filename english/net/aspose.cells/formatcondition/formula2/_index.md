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
// Called: Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
public void FormatCondition_Property_Formula2()
{
    Workbook wb = new Workbook();
    ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
    FormatConditionCollection fcc = cfc[cfc.Add()];
    fcc.Add(CellArea.CreateCellArea(0, 0, 1, 1),
        FormatConditionType.CellValue, OperatorType.Between, "abc def", "=\"a\"&\"b\"");
    FormatCondition fc = fcc[0];
    Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
    Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    fc = wb.Worksheets[0].ConditionalFormattings[0][0];
    Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
    Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
    wb = Util.ReSave(wb, SaveFormat.SpreadsheetML);
    fc = wb.Worksheets[0].ConditionalFormattings[0][0];
    Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
    Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
}
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


