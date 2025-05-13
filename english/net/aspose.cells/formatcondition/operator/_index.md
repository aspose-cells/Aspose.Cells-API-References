---
title: FormatCondition.Operator
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets the conditional format operator type
type: docs
url: /net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Gets and sets the conditional format operator type.

```csharp
public OperatorType Operator { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(fc.Operator, OperatorType.Between);
public void FormatCondition_Property_Operator()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    cells.InsertColumns(0, 4);
    Assert.AreEqual(cells["F2"].DoubleValue, 3);
    Assert.AreEqual(cells["H6"].DoubleValue, 5);
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
    Assert.AreEqual(fc.Formula1, "=F2=3");
    Assert.AreEqual(fc.Type, FormatConditionType.Expression);
    workbook.Save(Constants.destPath + "example.xls");

}
```

### See Also

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


