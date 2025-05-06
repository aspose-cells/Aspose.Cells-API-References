---
title: DeleteOptions.FormulaChangeMonitor
second_title: Aspose.Cells for .NET API Reference
description: DeleteOptions property. Gets/sets the monitor for tracking changes caused by the deletion
type: docs
url: /net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

Gets/sets the monitor for tracking changes caused by the deletion.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Examples

```csharp
// Called: cells.DeleteRows(2, 1, new DeleteOptions() { FormulaChangeMonitor = monitor });
[Test]
        public void Property_FormulaChangeMonitor()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 0].Formula = &quot;=A5&quot;;
            sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[0];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, &quot;=A8&gt;0&quot;, &quot;&quot;);
            FormulaChangeMonitorSimple monitor = new FormulaChangeMonitorSimple(wb);
            cells.DeleteRows(2, 1, new DeleteOptions() { FormulaChangeMonitor = monitor });
            Assert.AreEqual(&quot;0-0-0&quot;, monitor.mChangedCell, &quot;Changed cell&quot;);
            Assert.AreEqual(&quot;0-0-0&quot;, monitor.mFormatCondition, &quot;Changed format condition&quot;);
        }
```

### See Also

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


