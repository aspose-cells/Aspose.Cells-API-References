---
title: FormatConditionCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting
type: docs
url: /net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |

### Return Value

[0]:Formatting condition object index;[1] Effected cell rang index.

### Examples

```csharp
// Called: fcc.Add(CellArea.CreateCellArea(0, 0, 4, 0),
public void FormatConditionCollection_Method_Add()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    for (int i = 0; i < 5; i++)
    {
        cells[i, 0].PutValue(i);
    }
    ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
    FormatConditionCollection fcc = cfc[cfc.Add()];
    fcc.Add(CellArea.CreateCellArea(0, 0, 4, 0),
        FormatConditionType.Expression, OperatorType.None,
        "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)", null);
    int fontSize = wb.DefaultStyle.Font.Size;
    fcc[0].Style.Font.Size = fontSize + 2;
    for (int i = 0; i < 5; i++)
    {
        Assert.AreEqual(i < 3 ? fontSize : fontSize + 2,
            cells[i, 0].GetDisplayStyle().Font.Size, "Font size of A" + (i + 1));
    }
}
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


