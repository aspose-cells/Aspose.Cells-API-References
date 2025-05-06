---
title: CellArea.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the start column of this area
type: docs
url: /net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Gets or set the start column of this area.

```csharp
public int StartColumn;
```

### Examples

```csharp
// Called: ca.StartColumn = 0;
[Test]
        public void Field_StartColumn()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            //Adds an empty conditional formatting

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            //Sets the conditional format range.
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 0;
            ca.EndColumn = 0;
            fcs.AddArea(ca);
            ca = new CellArea();
            ca.StartRow = 1;
            ca.EndRow = 1;
            ca.StartColumn = 1;
            ca.EndColumn = 1;
            fcs.AddArea(ca);
            //Adds condition.
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.Between, &quot;0&quot;, &quot;100&quot;);
            //Adds condition.
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.Expression, OperatorType.Between, &quot;50&quot;, &quot;100&quot;);
            //Sets the background color.
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            checkFormatConditionType_Expression(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkFormatConditionType_Expression(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkFormatConditionType_Expression(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkFormatConditionType_Expression(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


