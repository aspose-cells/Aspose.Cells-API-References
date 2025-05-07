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
            Cells cells = wb.Worksheets.Add("Sheet2").Cells;
            cells[0, 0].Formula = "=Sheet1!A10";
            cells[0, 1].Formula = "=Sheet1!A5";
            cells[0, 2].Formula = "=A10";
            cells[0, 3].Formula = "=A5";
            cells = wb.Worksheets[0].Cells;
            cells[0, 0].Formula = "=A10";
            cells[0, 1].Formula = "=A5";

            DeleteOptions dopts = new DeleteOptions();
            HashSet<int> changed = new HashSet<int>();
            dopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            dopts.UpdateReference = true;
            cells.DeleteRows(6, 3, dopts);
            Assert.AreEqual(2, changed.Count, "Delete: Total changed cells");
            if (!changed.Contains(0))
            {
                Assert.Fail("Delete: Monitor should find Sheet1!A1 has been changed.");
            }
            if (!changed.Contains(1 << 24))
            {
                Assert.Fail("Delete: Monitor should find Sheet2!A1 has been changed.");
            }
            changed.Clear();
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            iopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            cells.InsertRows(6, 3, iopts);
            Assert.AreEqual(2, changed.Count, "Insert: Total changed cells");
            if (!changed.Contains(0))
            {
                Assert.Fail("Insert: Monitor should find Sheet1!A1 has been changed.");
            }
            if (!changed.Contains(1 << 24))
            {
                Assert.Fail("Insert: Monitor should find Sheet2!A1 has been changed.");
            }
        }
```

### See Also

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


