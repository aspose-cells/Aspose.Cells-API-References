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
// Called: fcc.Add(CellArea.CreateCellArea(2, 0, 2, 3),
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    cells[i, j].PutValue(i * 3 + j);
                }
            }
            sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[0];
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.ColorScale, OperatorType.None, null, null);
            fcc.Add(CellArea.CreateCellArea(2, 0, 2, 3),
                FormatConditionType.ColorScale, OperatorType.None, null, null);
            Assert.IsTrue(fcc[0].Priority > fcc[1].Priority,
                "Newly added format condition should have higher priorty than existing ones");
            wb = Util.ReSave(wb, SaveFormat.Excel97To2003);
            sheet = wb.Worksheets[0];
            Assert.AreEqual(1, sheet.ConditionalFormattings.Count, "ConditionalFormattings.Count");
            fcc = sheet.ConditionalFormattings[0];
            Assert.AreEqual(2, fcc.Count, "FormatConditionCollection.Count");
            Assert.AreEqual(FormatConditionType.ColorScale, fcc[0].Type, "FormatConditionCollection[0].Type");
            Assert.AreEqual(FormatConditionType.ColorScale, fcc[1].Type, "FormatConditionCollection[1].Type");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


