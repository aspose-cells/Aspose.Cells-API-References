---
title: "Cells.GetFirstDataRow"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cells 方法。获取指定列中包含数据的单元格的第一行索引"
type: docs
url: /zh/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

获取指定列中包含数据的单元格的第一行索引。

```csharp
public int GetFirstDataRow(int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | Int32 | 列索引。 |

### 返回值

首行索引。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据以演示该方法
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // 从工作表获取 Cells 集合
                Cells cells = worksheet.Cells;

                // 调用 GetFirstDataRow 获取列 A（索引 0）
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // 调用 GetFirstDataRow 获取列 B（索引 1）
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // 调用 GetFirstDataRow 获取列 C（索引 2）
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // 保存工作簿
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


