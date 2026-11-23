---
title: "Cell.IsCheckBoxStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 属性。指示是否将此单元格设置为复选框"
type: docs
url: /zh/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

指示是否将此单元格设置为复选框。

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问单元格 B1 并将其设置为复选框样式
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // 访问单元格 A1 并将其设置为带有值的复选框样式
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // 保存工作簿
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // 加载已保存的工作簿以验证属性
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // 验证 B1 为复选框样式
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // 将 B1 更改为非复选框样式并保存
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


