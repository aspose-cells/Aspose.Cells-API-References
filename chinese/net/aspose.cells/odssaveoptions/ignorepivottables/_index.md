---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "OdsSaveOptions 属性。指示是否保存数据透视表"
type: docs
url: /zh/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

指示是否保存数据透视表。

```csharp
public bool IgnorePivotTables { get; set; }
```

### 备注

OpenOffice 的数据透视表功能相比 Excel 设置更少，因此其数据透视表的结果有许多差异。有时在保存 .ods 文件时最好忽略这些数据透视表。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // 创建数据透视表
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 创建 OdsSaveOptions 实例
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // 显示当前 IgnorePivotTables 值
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // 设置为在保存时忽略数据透视表
            saveOptions.IgnorePivotTables = true;

            // 保存时忽略数据透视表
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // 设置为保存时包含数据透视表
            saveOptions.IgnorePivotTables = false;

            // 保存时包含数据透视表
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### 另请参见

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


