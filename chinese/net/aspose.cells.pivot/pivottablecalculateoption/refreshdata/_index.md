---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableCalculateOption 属性。指示是否刷新透视表的数据源"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

指示是否刷新数据透视表的数据源。

```csharp
public bool RefreshData { get; set; }
```

### 备注

如果为 true，则从数据源刷新透视缓存，然后基于相同的透视缓存计算所有透视表。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 设置透视表的示例数据
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 修改源数据
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // 使用 RefreshData 选项计算透视表
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // 输出更新后的透视表值
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### 另请参见

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


