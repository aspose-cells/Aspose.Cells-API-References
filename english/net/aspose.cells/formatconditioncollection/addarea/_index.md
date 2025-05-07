---
title: FormatConditionCollection.AddArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a conditional formatted cell range
type: docs
url: /net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Adds a conditional formatted cell range.

```csharp
public int AddArea(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |

### Return Value

Conditional formatted cell rang index.

### Examples

```csharp
// Called: fcs.AddArea(ca);
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            //Sets the conditional format range.
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 0;
            ca.EndColumn = 0;
            fcs.AddArea(ca);
            //Adds condition.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.LessThan, "10", "10");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            checkOperatorType_LessThan(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkOperatorType_LessThan(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkOperatorType_LessThan(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkOperatorType_LessThan(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


