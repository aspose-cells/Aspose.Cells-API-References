---
title: "SettableGlobalizationSettings.GetTableRowTypeOfAll"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取引用表中所有行组成的表行的类型名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofall/
---
## SettableGlobalizationSettings.GetTableRowTypeOfAll method

获取由引用表中的所有行组成的表行的类型名称。

```csharp
public override string GetTableRowTypeOfAll()
```

### 返回值

表行的类型名称

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfAll("EntireTable");
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"TableRowTypeOfAll: {rowType}");

                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["A3"].Value = "Banana";
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "A3", true)];

                Cell formulaCell = worksheet.Cells["B1"];
                formulaCell.Formula = "=COUNTA(Table1[#All])";
                Console.WriteLine($"Formula using #All: {formulaCell.Formula}");

                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfAll method: {ex.Message}");
            }
            
            workbook.Save("MethodGetTableRowTypeOfAllDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


