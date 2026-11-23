---
title: "Cells.GetMergedAreas"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cells 方法。获取所有合并的单元格"
type: docs
url: /zh/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

获取所有合并的单元格。

```csharp
public CellArea[] GetMergedAreas()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建一些合并单元格
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // 获取所有合并区域
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // 显示有关合并区域的信息
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### 另请参见

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


