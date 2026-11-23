---
title: "Cell.InsertText"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。向单元格插入一些字符。如果单元格是富格式化的，此方法可以保留原始格式。"
type: docs
url: /zh/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

向单元格插入一些字符。如果单元格是富格式化的，此方法可以保留原始格式。

```csharp
public void InsertText(int index, string text)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 索引。 |
| 文本 | String | 已插入的文本。 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问单元格 B3 并设置初始值
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // 在位置 6 插入文本
            cell.InsertText(6, "Inserted");
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


