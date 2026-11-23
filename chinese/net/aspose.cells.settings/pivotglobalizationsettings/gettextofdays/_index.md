---
title: "PivotGlobalizationSettings.GetTextOfDays"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 Days 的本地文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdays/
---
## PivotGlobalizationSettings.GetTextOfDays method

获取 "Days" 的本地文本。

```csharp
public virtual string GetTextOfDays()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(1500);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 将日期字段添加到行区域
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // 创建全局化设置
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // 演示 GetTextOfDays 方法
            Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());

            // 保存工作簿
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


