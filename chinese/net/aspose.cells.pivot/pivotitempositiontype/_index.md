---
title: "枚举 PivotItemPositionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotItemPositionType 枚举。表示在使用 ShowDataAs 计算时，基字段中透视基项的位置类型"
type: docs
url: /zh/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

表示在使用 ShowDataAs 计算时，基字段中枢基项的位置类型。

```csharp
public enum PivotItemPositionType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Previous | `0` | 表示 PivotField 中的前一个枢轴项。 |
| Next | `1` | 表示 PivotField 中的下一个枢轴项。 |
| Custom | `2` | 根据 PivotField 中枢轴项的索引，以不同的格式显示值。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 向工作簿添加新工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // 设置数据显示格式，使值显示为与前一个项的差异
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // 刷新并计算枢轴表
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存工作簿
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


