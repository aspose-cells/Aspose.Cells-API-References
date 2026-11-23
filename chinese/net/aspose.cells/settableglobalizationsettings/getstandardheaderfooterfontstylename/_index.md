---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的区域设置字体样式名称，获取用于页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

根据给定的区域设置字体样式名称获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localfontStyleName | String | 用于页眉/页脚的区域字体样式名称。 |

### 返回值

标准英文字体样式名称（常规、粗体、斜体）

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 设置标准页眉/页脚字体样式名称映射
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 使用本地区域字体样式名称调用 GetStandardHeaderFooterFontStyleName 方法
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // 显示结果
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // 使用本地区域字体样式名称创建页眉
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // 在电子表格中显示效果
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


