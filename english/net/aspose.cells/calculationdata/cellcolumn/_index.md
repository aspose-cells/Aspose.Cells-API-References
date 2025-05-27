---
title: CalculationData.CellColumn
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the column index of the cell where the function is in
type: docs
url: /net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Gets the column index of the cell where the function is in.

```csharp
public int CellColumn { get; }
```

### Examples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellColumnDemo
    {
        private Dictionary<int, object> _values = new Dictionary<int, object>();

        public void CalculationData_Property_CellColumn(CalculationData data)
        {
            if (_values == null)
            {
                throw new Exception("Custom implementation to ignore calculation of formula with function "
                    + data.FunctionName);
            }
            _values[data.CellColumn] = data.CalculatedValue;
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calculate formulas
            workbook.CalculateFormula();

            // Create instance and demonstrate CellColumn usage
            var demo = new CalculationDataPropertyCellColumnDemo();
            
            // Create mock CalculationData since we can't instantiate it directly
            var cell = worksheet.Cells["A3"];
            var data = new CalculationData
            {
                Cell = cell,
                CalculatedValue = cell.Value
            };
            
            demo.CalculationData_Property_CellColumn(data);

            // Output the stored value
            Console.WriteLine("Stored value for column {0}: {1}", 
                data.CellColumn, demo._values[data.CellColumn]);
        }
    }

    // Mock CalculationData class since we can't instantiate the real one
    public class CalculationData
    {
        public Cell Cell { get; set; }
        public object CalculatedValue { get; set; }
        public string FunctionName => "";
        public int CellColumn => Cell?.Column ?? -1;
    }
}
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


