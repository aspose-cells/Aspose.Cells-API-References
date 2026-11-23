---
title: "Row.GetCellByIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Row 方法。根据此行单元格集合中的特定索引获取单元格"
type: docs
url: /zh/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

根据此行单元格集合中的特定索引获取单元格。

```csharp
public Cell GetCellByIndex(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 此行单元格集合中单元格的索引（位置）。 |

### 返回值

给定位置的 Cell 对象。

### 备注

若要顺序遍历所有单元格且不进行修改，使用 [`GetEnumerator`](../getenumerator/) 的性能优于逐个使用此方法获取单元格。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向第一行的单元格添加数据
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // 获取第一行
            Row row = worksheet.Cells.Rows[0];

            // 演示使用 Int32 参数的 GetCellByIndex
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


