---
title: "Cell.ToJson"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。将 Cell 转换为 JSON 结构数据"
type: docs
url: /zh/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

将 [`Cell`](../) 转换为 JSON 结构数据。

```csharp
public string ToJson()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 设置示例数据和样式
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // 获取单元格并转换为 JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // 输出 JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


