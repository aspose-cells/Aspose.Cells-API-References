---
title: "SettableGlobalizationSettings.GetTableRowTypeOfData"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取由引用表的数据区域组成的表行的类型名称。默认是 Data，因此在公式中 Data 表示表的数据区域"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/
---
## SettableGlobalizationSettings.GetTableRowTypeOfData method

获取由引用表的数据区域组成的表行的类型名称。默认是 "Data"，因此在公式中 "#Data" 代表表格的数据区域。

```csharp
public override string GetTableRowTypeOfData()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
                settings.SetTableRowTypeOfData("CustomData");
                string rowType = settings.GetTableRowTypeOfData();
                Console.WriteLine($"TableRowTypeOfData: {rowType}");

                workbook.Settings.GlobalizationSettings = settings;

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["B2"].PutValue(5.5);
                worksheet.Cells["B3"].PutValue(3.8);

                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "Inventory"; // Changed from Name to DisplayName
                
                worksheet.Cells["B4"].Formula = "=SUM(Inventory[#CustomData][Price])";
                
                workbook.CalculateFormula();
                Console.WriteLine($"Total price: {worksheet.Cells["B4"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


