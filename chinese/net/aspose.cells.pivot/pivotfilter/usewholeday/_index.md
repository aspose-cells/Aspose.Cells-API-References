---
title: "PivotFilter.UseWholeDay"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilter 属性。指示其日期过滤条件是否使用整天"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfilter/usewholeday/
---
## PivotFilter.UseWholeDay property

指示其日期过滤条件是否使用整天。

```csharp
public bool UseWholeDay { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyUseWholeDayDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // 创建示例数据
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Amount";
            cells["A2"].Value = new DateTime(2023, 1, 15);
            cells["A3"].Value = new DateTime(2023, 1, 20);
            cells["A4"].Value = new DateTime(2023, 2, 5);
            cells["A5"].Value = new DateTime(2023, 2, 10);
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // 创建数据透视表
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "H3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount field
            
            // 添加透视过滤器
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.DateBetween);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.Value1 = "2023-01-01";
            filter.Value2 = "2023-01-31";
            
            // 设置并演示 UseWholeDay 属性
            filter.UseWholeDay = true;
            Console.WriteLine($"UseWholeDay value after setting: {filter.UseWholeDay}");

            // 保存工作簿
            workbook.Save("PivotFilterUseWholeDayDemo.xlsx");
            
            // 重新加载以验证持久性
            Workbook verifyWorkbook = new Workbook("PivotFilterUseWholeDayDemo.xlsx");
            PivotTable verifyPivot = verifyWorkbook.Worksheets[0].PivotTables[0];
            PivotFilter verifyFilter = verifyPivot.PivotFilters[0];
            Console.WriteLine($"UseWholeDay value after reloading: {verifyFilter.UseWholeDay}");
        }
    }
}
```

### 另请参见

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


