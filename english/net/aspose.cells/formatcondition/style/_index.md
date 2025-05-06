---
title: FormatCondition.Style
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets or setts style of conditional formatted cell ranges
type: docs
url: /net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Gets or setts style of conditional formatted cell ranges.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: fc4.Style.Font.Size = 21;
[Test]
        public void Property_Style() //CELLSNET-48190
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[2, 2];
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 2, 2));
            FormatCondition fc1 = fcc[fcc.AddCondition(FormatConditionType.CellValue)];
            fc1.Operator = OperatorType.GreaterThan;
            fc1.Formula1 = &quot;-5&quot;;
            fc1.Style.Font.Size = 5;
            Assert.AreEqual(5, cell.GetDisplayStyle().Font.Size, &quot;First cond has been added&quot;);

            FormatCondition fc2 = fcc[fcc.AddCondition(FormatConditionType.CellValue)];
            fc2.Operator = OperatorType.LessThan;
            fc2.Formula1 = &quot;2&quot;;
            fc2.Style.Font.Size = 6;
            Assert.AreEqual(6, cell.GetDisplayStyle().Font.Size, &quot;Second cond has been added&quot;);
            if (fc2.Priority &gt;= fc1.Priority)
            {
                Assert.Fail(&quot;Priority values order should be fc2&lt;fc1&quot;);
            }

            fc2.Priority = fc1.Priority + 1;
            Assert.AreEqual(5, cell.GetDisplayStyle().Font.Size,
                &quot;Priority has been changed manually for the second cond&quot;);

            FormatCondition fc3 = fcc[fcc.AddCondition(FormatConditionType.CellValue)];
            fc3.Operator = OperatorType.LessThan;
            fc3.Formula1 = &quot;1&quot;;
            fc3.Style.Font.Size = 7;
            Assert.AreEqual(7, cell.GetDisplayStyle().Font.Size, &quot;Third cond has been added&quot;);
            if (fc3.Priority &gt;= fc1.Priority || fc1.Priority &gt;= fc2.Priority)
            {
                Assert.Fail(&quot;Priority values order should be fc3&lt;fc1&lt;fc2&quot;);
            }
            fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(2, 2, 3, 3));
            FormatCondition fc4 = fcc[fcc.AddCondition(FormatConditionType.CellValue)];
            fc4.Operator = OperatorType.GreaterThan;
            fc4.Formula1 = &quot;-3&quot;;
            fc4.Style.Font.Size = 21;
            Assert.AreEqual(21, cell.GetDisplayStyle().Font.Size, &quot;Forth cond has been added&quot;);
            if (fc4.Priority &gt;= fc3.Priority || fc3.Priority &gt;= fc1.Priority || fc1.Priority &gt;= fc2.Priority)
            {
                Assert.Fail(&quot;Priority values order should be fc4&lt;fc3&lt;fc1&lt;fc2&quot;);
            }

            fc4.Priority = fc2.Priority + 1;
            Assert.AreEqual(7, cell.GetDisplayStyle().Font.Size,
                &quot;Priority has been changed manually for the forth cond&quot;);

            FormatCondition fc5 = fcc[fcc.AddCondition(FormatConditionType.CellValue)];
            fc5.Operator = OperatorType.GreaterThan;
            fc5.Formula1 = &quot;-1&quot;;
            fc5.Style.Font.Size = 22;
            Assert.AreEqual(22, cell.GetDisplayStyle().Font.Size, &quot;Fifth cond&quot;);
            if (fc5.Priority &gt;= fc3.Priority || fc3.Priority &gt;= fc1.Priority
                || fc1.Priority &gt;= fc2.Priority || fc2.Priority &gt;= fc4.Priority)
            {
                Assert.Fail(&quot;Priority values order should be fc5&lt;fc3&lt;fc1&lt;fc2&lt;fc4&quot;);
            }
        }
```

### See Also

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


