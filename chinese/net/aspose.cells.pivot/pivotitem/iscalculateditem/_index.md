---
title: "PivotItem.IsCalculatedItem"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotItem 属性。指示此数据透视项是否为计算公式项"
type: docs
url: /zh/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

指示此数据透视项是否为计算公式项。

```csharp
public bool IsCalculatedItem { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 计算数据透视表数据
            pivotTable.CalculateData();

            // 从第一个数据透视字段获取第一个数据透视项
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // 显示 IsCalculatedItem 属性值
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // 检查数据透视项是否为计算项
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // 保存工作簿
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


