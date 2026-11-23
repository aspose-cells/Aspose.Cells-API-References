---
title: "PivotField.GetFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。获取计算字段的公式。仅适用于计算字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

获取计算字段的公式。仅适用于计算字段。

```csharp
public string GetFormula()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 添加具有公式的计算字段
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // 从计算字段获取公式
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // 输出公式
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


