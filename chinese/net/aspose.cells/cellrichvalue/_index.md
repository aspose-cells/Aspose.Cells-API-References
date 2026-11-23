---
title: "类 CellRichValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.CellRichValue 类。表示单元格的富值"
type: docs
url: /zh/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

表示单元格的富值。

```csharp
public abstract class CellRichValue
```

## 属性

| 名称 | 描述 |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | 获取与图像关联的替代文本。 |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | 获取单元格的错误值类型。 |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | 获取单元格的图像数据。 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在单元格 A1 中设置富值
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // 从单元格 A1 获取富值
            CellRichValue richValue = cell.GetRichValue();
            
            // 显示富值属性
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // 保存工作簿
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


