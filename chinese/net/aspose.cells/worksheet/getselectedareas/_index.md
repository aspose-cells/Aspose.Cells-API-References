---
title: "Worksheet.GetSelectedAreas"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Worksheet 方法。获取设计器电子表格中选定的单元格范围"
type: docs
url: /zh/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

获取设计器电子表格中选定的单元格范围。

```csharp
public Range[] GetSelectedAreas()
```

### 返回值

返回所有选定的范围。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 选择多个范围
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // 获取选定的区域
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // 显示有关选定区域的信息
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // 清除选择并选择单个范围
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // 获取单个选定的区域
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### 另请参见

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


