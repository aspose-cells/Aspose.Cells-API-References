---
title: "Cell.SetTableFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。为给定范围创建双变量数据表，从此单元格开始"
type: docs
url: /zh/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

为给定范围创建双变量数据表，从此单元格开始。

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | Int32 | 用于填充公式的行数。 |
| columnNumber | Int32 | 用于填充公式的列数。 |
| rowInputCell | String | 行输入单元格 |
| columnInputCell | String | 列输入单元格 |
| 值 | Object[][] | 表格公式范围内单元格的值 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // 将设置表格公式的目标单元格
            Cell targetCell = worksheet.Cells["C3"];

            // 准备 SetTableFormula 的参数
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // 在目标单元格上设置表格公式
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // 计算工作簿公式以刷新结果
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

为给定范围创建单变量数据表，从此单元格开始。

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | Int32 | 用于填充公式的行数。 |
| columnNumber | Int32 | 用于填充公式的列数。 |
| inputCell | String | 输入单元格 |
| isRowInput | 布尔 | 指示输入单元格是行输入单元格（true）还是列输入单元格（false）。 |
| 值 | Object[][] | 表格公式范围内单元格的值 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // 准备 SetTableFormula 的参数
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // 获取数据表的目标单元格（C3）
                Cell tableCell = worksheet.Cells["C3"];
                // 使用利率变化调用 SetTableFormula
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // 计算公式以刷新表格结果
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

为给定范围创建双变量数据表，从此单元格开始。

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | Int32 | 用于填充公式的行数。 |
| columnNumber | Int32 | 用于填充公式的列数。 |
| rowIndexOfRowInputCell | Int32 | 行输入单元格的行索引 |
| columnIndexOfRowInputCell | Int32 | 行输入单元格的列索引 |
| rowIndexOfColumnInputCell | Int32 | 列输入单元格的行索引 |
| columnIndexOfColumnInputCell | Int32 | 列输入单元格的列索引 |
| 值 | Object[][] | 表格公式范围内单元格的值 |

### 示例

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
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // 准备数据表的输入值（利率和贷款金额）
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // 使用 3x3 数据表维度和输入单元格偏移设置表格公式
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
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

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

为给定范围创建单变量数据表，从此单元格开始。

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNumber | Int32 | 用于填充公式的行数。 |
| columnNumber | Int32 | 用于填充公式的列数。 |
| rowIndexOfInputCell | Int32 | 输入单元格的行索引 |
| columnIndexOfInputCell | Int32 | 输入单元格的列索引 |
| isRowInput | 布尔 | 指示输入单元格是行输入单元格（true）还是列输入单元格（false）。 |
| 值 | Object[][] | 表格公式范围内单元格的值 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // 创建表格公式参数的示例数据数组
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // 获取用于应用表格公式的目标单元格
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // 设置表格公式，使用：
                // 3 行，2 列，输入单元格位于 A1 (0,0)，
                // 行输入类型，以及示例值
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


