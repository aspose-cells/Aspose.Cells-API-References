---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。获取此数据透视表的水平分页符"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

获取此数据透视表的水平分页符。

```csharp
public int[] GetHorizontalPageBreaks()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // 从源文件创建工作簿
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问第一个数据透视表
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 刷新并计算数据透视表数据
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // 获取水平分页符
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // 显示结果
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


