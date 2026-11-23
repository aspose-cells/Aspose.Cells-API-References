---
title: "PivotField.RegionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。指定此字段在透视表中显示的区域"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

指定此字段在透视表中显示的区域。

```csharp
public PivotFieldType RegionType { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 刷新透视表数据
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 获取第一个透视字段
            PivotField pivotField = pivotTable.RowFields[0];

            // 显示当前 RegionType 值
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // 演示如何使用 RegionType 属性
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // 保存工作簿
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


