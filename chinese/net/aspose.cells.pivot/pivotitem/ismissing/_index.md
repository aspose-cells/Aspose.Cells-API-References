---
title: "PivotItem.IsMissing"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotItem 属性。指示该项是否已从数据源中移除"
type: docs
url: /zh/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

指示该项是否已从数据源中移除。

```csharp
public bool IsMissing { get; }
```

### 备注

True 表示此值已从数据源中移除。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 刷新透视表数据
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 获取第一行字段中的第一个透视项
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // 显示 IsMissing 属性值
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // 创建一个可能缺少项的场景
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 检查原始透视项是否已缺失
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // 保存工作簿
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


