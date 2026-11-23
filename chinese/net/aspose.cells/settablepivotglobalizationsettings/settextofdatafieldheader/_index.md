---
title: "SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。设置数据透视表中值区域字段标题的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

设置 PivotTable 中值区域字段标题的文本。

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | String | 数据字段标题名称的文本 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // 创建 SettablePivotGlobalizationSettings 的实例
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // 设置数据字段标题的自定义文本
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // 通过获取当前文本来验证更改
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // 保存工作簿以演示成功执行
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


