---
title: "GlobalizationSettings.PivotSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GlobalizationSettings 属性。获取或设置数据透视表的全局化设置"
type: docs
url: /zh/net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

获取或设置数据透视表的全局化设置。

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfTotal()
        {
            return "Custom Total";
        }

        public override string GetTextOfGrandTotal()
        {
            return "Custom Grand Total";
        }

        public override string GetTextOfDataFieldHeader()
        {
            return "DataCaption";
        }

        public override string GetTextOfProtectedName(string protectedName)
        {
            return protectedName + "2";
        }
    }

    public class GlobalizationSettingsPropertyPivotSettingsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加示例数据
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Orange");
            dataSheet.Cells["B3"].PutValue(2000);

            // 创建数据透视表
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];
            
            // 添加行字段和数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 为数据透视表设置自定义全局化设置
            CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;

            // 刷新数据透视表以应用设置
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存工作簿
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


