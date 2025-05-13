---
title: Enum FormatConditionValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FormatConditionValueType enum. Condition value type
type: docs
url: /net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Condition value type.

```csharp
public enum FormatConditionValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Formula | `0` | The minimum/ midpoint / maximum value for the gradient is determined by a formula. |
| Max | `1` | Indicates that the maximum value in the range shall be used as the maximum value for the gradient. |
| Min | `2` | Indicates that the minimum value in the range shall be used as the minimum value for the gradient. |
| Number | `3` | Indicates that the minimum / midpoint / maximum value for the gradient is specified by a constant numeric value. |
| Percent | `4` | Value indicates a percentage between the minimum and maximum values in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| Percentile | `5` | Value indicates a percentile ranking in the range shall be used as the minimum / midpoint / maximum value for the gradient. |
| AutomaticMax | `6` | Indicates that the Automatic maximum value in the range shall be used as the Automatic maximum value for the gradient. |
| AutomaticMin | `7` | Indicates that the Automatic minimum value in the range shall be used as the Automatic minimum value for the gradient. |

### Examples

```csharp
// Called: FormatConditionValueType fcvType = fc.IconSet.Cfvos[0].Type;
public void Cells_Type_FormatConditionValueType()
{
    //String filePath = Constants.destPath + "Test3Conditionaldest.xlsx";
    Workbook _book = new Workbook();
    Worksheet _sheet = _book.Worksheets[0];
    //write
    FormatConditionCollection conds = GetFormatCondition("M1:O2", Color.AliceBlue, _sheet);
    int idx = conds.AddCondition(FormatConditionType.IconSet);
    FormatCondition cond = conds[idx];
    cond.IconSet.Type = IconSetType.Boxes5;
    cond.IconSet.ShowValue = false;
    cond.IconSet.Reverse = true;
    Cell c = _sheet.Cells["M1"];
    c.PutValue("Boxes5");

    //_book.Save(filePath, SaveFormat.Xlsx);
    //read
    _book = Util.ReSave(_book, SaveFormat.Xlsx);// new Workbook(filePath);
    _sheet = _book.Worksheets[0];
    //
    FormatConditionCollection fcs = _sheet.ConditionalFormattings[0];
    FormatCondition fc = null;
    if (fcs.Count > 0)
        fc = fcs[0];

    string fcvalue = "";
    int priority;
    object val = null;
    string sqref = "";
    bool showValue, reverse;
    FormatConditionType fcType = fc.Type;
    IconSetType iconType = fc.IconSet.Type;
    FormatConditionValueType fcvType = fc.IconSet.Cfvos[0].Type;
    priority = fc.Priority;
    showValue = fc.IconSet.ShowValue;
    reverse = fc.IconSet.Reverse;

    Assert.AreEqual(priority, 1);
    Assert.AreEqual(fcType, FormatConditionType.IconSet);
    Assert.AreEqual(iconType, IconSetType.Boxes5);
    Assert.AreEqual(fcvType, FormatConditionValueType.Percent);
    int count = fc.IconSet.Cfvos.Count;
    string[] vals = new string[] { "0", "20", "40", "60", "80" };
    for (int i = 0; i < count; i++)
    {
        val = fc.IconSet.Cfvos[i].Value;
        fcvalue = val.ToString();
        Assert.AreEqual(fcvalue, vals[i]);
    }
    Assert.AreEqual(showValue, false);
    Assert.AreEqual(reverse, true);
    CellArea cellare = fcs.GetCellArea(0);
    sqref = GetCellAreaName(cellare);
    Assert.AreEqual(sqref, "M1:O2");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


