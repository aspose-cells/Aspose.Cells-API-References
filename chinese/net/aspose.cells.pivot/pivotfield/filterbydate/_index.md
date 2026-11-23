---
title: "PivotField.FilterByDate"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。按行或列透视字段的日期值进行筛选"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

按行或列透视字段的日期值进行筛选。

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | PivotFilterType | 过滤数据的类型。 |
| dateTime1 | DateTime | 过滤条件的日期标签 |
| dateTime2 | DateTime | 介于过滤条件的上限日期标签 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加带日期的示例数据
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 将日期字段添加到列区域
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // 应用日期筛选（2020-2021 年之间的 9 月日期）
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // 刷新并计算数据透视表
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // 保存结果
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


