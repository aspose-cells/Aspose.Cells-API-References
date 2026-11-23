---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 属性。指示在更新时是否自动调整列宽"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

指示在更新时是否自动调整列宽

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问包含数据透视表的工作表
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // 访问数据透视表
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 在更新时禁用自动适应列宽
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // 刷新数据透视表以应用更改
            worksheet.RefreshPivotTables();
            
            // 保存工作簿
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


