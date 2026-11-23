---
title: "PivotTable.ShowDetail"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。将数据区域中某项的详细信息显示到新表中"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

将数据区域中某项的详细信息显示到新表中。

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | Int32 | 偏移到数据区域中的第一数据行。 |
| columnOffset | Int32 | 偏移到数据区域中的第一数据列。 |
| newSheet | 布尔 | 将详细信息显示到新工作表中。 |
| destRow | Int32 | 目标行。 |
| destColumn | Int32 | 目标列。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // 显示特定单元格的详细信息
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // 保存工作簿
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


