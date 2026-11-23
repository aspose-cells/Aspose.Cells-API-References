---
title: "PivotItem.IsDetailHidden"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotItem 属性。获取和设置此透视项的详细信息是否隐藏"
type: docs
url: /zh/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

获取和设置此透视项的详细信息是否隐藏。

```csharp
public bool IsDetailHidden { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // 为数据透视表添加示例数据
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // 刷新并计算数据
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 隐藏 "Fruit" 类别的详细信息
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // 保存工作簿
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


