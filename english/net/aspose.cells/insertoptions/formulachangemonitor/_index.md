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
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MyCellChangeMonitor
    {
        private HashSet<int> changedCells;

        public MyCellChangeMonitor(HashSet<int> changed)
        {
            changedCells = changed;
        }

        public void OnChange(int sheetIndex, int rowIndex, int colIndex)
        {
            changedCells.Add((sheetIndex << 24) | (rowIndex << 8) | colIndex);
        }
    }

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Set up formulas that will be affected by row insertion
            cells["A1"].Formula = "=A10";
            cells["B1"].Formula = "=A5";

            // Create InsertOptions with FormulaChangeMonitor
            InsertOptions iopts = new InsertOptions();
            HashSet<int> changedCells = new HashSet<int>();
            var monitor = new MyCellChangeMonitor(changedCells);
            
            // Using reflection to set FormulaChangeMonitor if the property exists
            var prop = typeof(InsertOptions).GetProperty("FormulaChangeMonitor");
            if (prop != null)
            {
                prop.SetValue(iopts, monitor);
            }
            
            iopts.UpdateReference = true;

            // Insert rows which will affect the formulas
            cells.InsertRows(5, 3, iopts);

            // Output the changed cells
            Console.WriteLine("Changed cells count: " + changedCells.Count);
            foreach (int cell in changedCells)
            {
                int sheetIndex = cell >> 24;
                int rowIndex = (cell >> 8) & 0xFFFF;
                int colIndex = cell & 0xFF;
                Console.WriteLine($"Sheet {sheetIndex}, Cell [{rowIndex},{colIndex}] was changed");
            }
        }
    }
}
```

### See Also

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


