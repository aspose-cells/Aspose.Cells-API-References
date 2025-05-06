---
title: InsertOptions.FormulaChangeMonitor
second_title: Aspose.Cells for .NET API Reference
description: InsertOptions property. Gets/sets the monitor for tracking changes caused by the insertion
type: docs
url: /net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Gets/sets the monitor for tracking changes caused by the insertion.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Examples

```csharp
// Called: iopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
[Test]
        public void Property_FormulaChangeMonitor()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            cells[0, 0].Formula = &quot;=Sheet1!A10&quot;;
            cells[0, 1].Formula = &quot;=Sheet1!A5&quot;;
            cells[0, 2].Formula = &quot;=A10&quot;;
            cells[0, 3].Formula = &quot;=A5&quot;;
            cells = wb.Worksheets[0].Cells;
            cells[0, 0].Formula = &quot;=A10&quot;;
            cells[0, 1].Formula = &quot;=A5&quot;;

            DeleteOptions dopts = new DeleteOptions();
            HashSet&lt;int&gt; changed = new HashSet&lt;int&gt;();
            dopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            dopts.UpdateReference = true;
            cells.DeleteRows(6, 3, dopts);
            Assert.AreEqual(2, changed.Count, &quot;Delete: Total changed cells&quot;);
            if (!changed.Contains(0))
            {
                Assert.Fail(&quot;Delete: Monitor should find Sheet1!A1 has been changed.&quot;);
            }
            if (!changed.Contains(1 &lt;&lt; 24))
            {
                Assert.Fail(&quot;Delete: Monitor should find Sheet2!A1 has been changed.&quot;);
            }
            changed.Clear();
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            iopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            cells.InsertRows(6, 3, iopts);
            Assert.AreEqual(2, changed.Count, &quot;Insert: Total changed cells&quot;);
            if (!changed.Contains(0))
            {
                Assert.Fail(&quot;Insert: Monitor should find Sheet1!A1 has been changed.&quot;);
            }
            if (!changed.Contains(1 &lt;&lt; 24))
            {
                Assert.Fail(&quot;Insert: Monitor should find Sheet2!A1 has been changed.&quot;);
            }
        }
```

### See Also

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


