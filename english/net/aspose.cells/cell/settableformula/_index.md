---
title: Cell.SetTableFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Create twovariable data table for given range starting from this cell
type: docs
url: /net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Create two-variable data table for given range starting from this cell.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowInputCell | String | the row input cell |
| columnInputCell | String | the column input cell |
| values | Object[][] | values for cells in table formula range |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set initial values for input cells
            worksheet.Cells["B1"].PutValue(2);  // Row input cell
            worksheet.Cells["B2"].PutValue(3);  // Column input cell

            // Target cell where table formula will be set
            Cell targetCell = worksheet.Cells["D1"];

            // Prepare parameters for SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "B1";
            string columnInputCell = "B2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Set the table formula on the target cell
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Calculate workbook formulas to refresh results
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Create one-variable data table for given range starting from this cell.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| inputCell | String | the input cell |
| isRowInput | Boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setup base values for PMT calculation
            worksheet.Cells["B1"].PutValue(100000);  // Loan amount
            worksheet.Cells["B2"].PutValue(0.05);    // Annual interest rate
            worksheet.Cells["B3"].PutValue(360);     // Term in months

            // Create PMT formula in B4
            Cell formulaCell = worksheet.Cells["B4"];
            formulaCell.Formula = "=PMT(B2/12, B3, B1)";
            
            try
            {
                // Prepare parameters for SetTableFormula
                int rowCount = 5;
                int colCount = 1;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.04 },
                    new object[] { 0.045 },
                    new object[] { 0.05 },
                    new object[] { 0.055 },
                    new object[] { 0.06 }
                };

                // Get target cell for data table (D1)
                Cell tableCell = worksheet.Cells["D1"];
                
                // Call SetTableFormula with interest rate variations
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "B2",
                    isRowInput: true,
                    values: inputValues
                );

                // Calculate formulas to refresh table results
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Create two-variable data table for given range starting from this cell.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | Int32 | row index of the row input cell |
| columnIndexOfRowInputCell | Int32 | column index of the row input cell |
| rowIndexOfColumnInputCell | Int32 | row index of the column input cell |
| columnIndexOfColumnInputCell | Int32 | column index of the column input cell |
| values | Object[][] | values for cells in table formula range |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setup base formula and input cells
            Cell formulaCell = worksheet.Cells["B2"];
            formulaCell.Formula = "=PMT(B1/12, 60, A2)";

            // Prepare input values for data table (interest rates and loan amounts)
            object[][] tableValues = new object[2][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };  // Row input values
            tableValues[1] = new object[] { 10000, 20000, 30000 }; // Column input values

            try
            {
                // Set table formula with 3x3 data table dimensions and input cell offsets
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: -1,  // B1 (1 row above formula cell)
                    columnIndexOfRowInputCell: 0,   // Same column as formula cell
                    rowIndexOfColumnInputCell: 0,   // Same row as formula cell
                    columnIndexOfColumnInputCell: -1, // A2 (1 column left of formula cell)
                    values: tableValues
                );

                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Create one-variable data table for given range starting from this cell.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowIndexOfInputCell | Int32 | row index of the input cell |
| columnIndexOfInputCell | Int32 | column index of the input cell |
| isRowInput | Boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set base value in input cell (A1)
            worksheet.Cells["A1"].PutValue(50);

            // Create sample data array for table formula parameters
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Get target cell to apply table formula
            Cell formulaCell = worksheet.Cells["C7"];

            try
            {
                // Set table formula with: 
                // 3 rows, 2 columns, input cell at A1 (0,0), 
                // row input type, and sample values
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C7.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


