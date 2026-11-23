---
title: "SettableGlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取由表头组成的表行的类型名称。默认是 Headers，因此在公式中 Headers 代表表头。"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/
---
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method

获取由表头组成的表行的类型名称。默认是 "Headers"，因此在公式中 "#Headers" 代表表头。

```csharp
public override string GetTableRowTypeOfHeaders()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfHeaders("CustomHeaders");
            workbook.Settings.GlobalizationSettings = settings;

            // 创建示例表数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            try
            {
                // 获取表头的表行类型
                string rowType = settings.GetTableRowTypeOfHeaders();
                Console.WriteLine($"Table row type for headers: {rowType}");

                // 创建 ListObject（表）
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

                // 在公式中使用自定义的页眉引用
                worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
                Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);

                // 计算公式
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


