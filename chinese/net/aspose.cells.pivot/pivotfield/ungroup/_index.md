---
title: "PivotField.Ungroup"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。取消对透视字段的分组"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

取消对透视字段的分组。

```csharp
public void Ungroup()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问第一个数据透视表
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 取消对第一列字段的分组
            pivotTable.ColumnFields[0].Ungroup();
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


