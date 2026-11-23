---
title: "PivotFilter.GetTop10Value"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilter 方法。获取过滤器的前 10 设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

获取过滤器的前10项设置。

```csharp
public Top10Filter GetTop10Value()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问第一个工作表和数据透视表
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 在第一个基础字段上应用前10过滤器（按计数显示前2项）
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // 获取已应用的过滤器及其前10个值
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // 输出过滤器详细信息
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


