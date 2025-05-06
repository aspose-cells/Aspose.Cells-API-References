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
// Called: fc2.Formula1 = fmls2[0];
[Test]
        public void Property_Formula1()
        {
            Workbook wb = new Workbook();
            int v0 = wb.DefaultStyle.Font.Size;
            int v1 = v0 + 5;
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 10; i++)
            {
                cells[i, 2].PutValue(i + 1);
            }
            string[] fmls1 = new string[] { &quot;=C5&gt;0&quot; };
            string[] fmls2 = new string[] { &quot;=SUM(C5:C10)&gt;0&quot; };
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 0, 0));
            FormatCondition fc1 = fcc[fcc.AddCondition(FormatConditionType.Expression)];
            fc1.Formula1 = fmls1[0];
            fc1.Style.Font.Size = v1;
            fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(1, 0, 1, 0));
            FormatCondition fc2 = fcc[fcc.AddCondition(FormatConditionType.Expression)];
            fc2.Formula1 = fmls2[0];
            fc2.Style.Font.Size = v1;
            CheckCellFormatConditions(cells[0, 0], v1, fmls1, &quot;With original conditional formatting,&quot;);
            CheckCellFormatConditions(cells[1, 0], v1, fmls2, &quot;With original conditional formatting,&quot;);
            cells.DeleteRow(4);
            CheckEmptyAppliedRange(cfc, &quot;After deleting row,&quot;);
            fmls1[0] = &quot;=#REF!&gt;0&quot;;
            fmls2[0] = &quot;=SUM(C5:C9)&gt;0&quot;;
            CheckCellFormatConditions(cells[0, 0], v0, fmls1, &quot;After deleting row,&quot;);
            CheckCellFormatConditions(cells[1, 0], v1, fmls2, &quot;After deleting row,&quot;);
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


