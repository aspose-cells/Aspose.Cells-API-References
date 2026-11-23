---
title: "PivotTable.MoveTo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。将数据透视表移动到工作表中的其他位置"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

将数据透视表移动到工作表中的其他位置。

```csharp
public void MoveTo(int row, int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 行索引。 |
| 列 | Int32 | 列索引。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // 计算用于填充数据透视表的数据
            pivotTable.CalculateData();

            try
            {
                // 调用 MoveTo 方法并使用 (Int32, Int32) 参数来移动数据透视表
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // 再次计算数据以更新已移动的数据透视表
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(int, int, int) {#moveto_1}

将数据透视表移动到工作表中的其他位置。

```csharp
public void MoveTo(int sheetIndex, int row, int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | Int32 | 目标工作表的索引 |
| 行 | Int32 | 行索引。 |
| 列 | Int32 | 列索引。 |

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_2}

将数据透视表移动到工作表中的其他位置。

```csharp
public void MoveTo(string destCellName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destCellName | String | 目标单元格名称。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodMoveToWithStringDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // 设置示例数据
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // 创建数据透视表
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            
            // 向数据透视表添加字段
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // 设置样式并刷新
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            sheet.RefreshPivotTables();

            // 将数据透视表移动到新位置
            pivot.MoveTo("H16");
            sheet.RefreshPivotTables();

            // 保存工作簿
            book.Save("PivotTableMoveToExample.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


