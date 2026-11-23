---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取单元格错误值的显示字符串"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

获取单元格错误值的显示字符串。

```csharp
public override string GetErrorValueString(string err)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 错误 | String | 错误值，例如 #VALUE!、#NAME? |

### 返回值

默认情况下返回错误值本身

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // 创建一个带错误值的单元格
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // 使用错误值字符串调用 GetErrorValueString
                string errorString = settings.GetErrorValueString("#N/A");
                
                // 显示结果
                Console.WriteLine("Error value string: " + errorString);

                // 通过将另一个单元格的值设置为返回的字符串来显示效果
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


