---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotAreaFilter 方法。获取此过滤器设置了哪种小计"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

获取为此过滤器设置的汇总方式。

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | 小计函数类型。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 添加透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段并配置小计
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // 创建透视区域并检查小计设置
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // 演示 IsSubtotalSet 的用法
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // 保存工作簿
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


