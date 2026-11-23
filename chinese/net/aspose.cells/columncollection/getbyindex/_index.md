---
title: "ColumnCollection.GetByIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ColumnCollection 方法。通过索引获取列对象"
type: docs
url: /zh/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

通过索引获取列对象。

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 |  |

### 返回值

返回列对象。

### 备注

注意：此成员现已过时。请改用 Columns.GetColumnByIndex() 方法。此属性将在自 2010 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 通过设置宽度在集合中创建列
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // 从 ColumnCollection 获取第二列（索引 1）
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // 修改检索到的列
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


