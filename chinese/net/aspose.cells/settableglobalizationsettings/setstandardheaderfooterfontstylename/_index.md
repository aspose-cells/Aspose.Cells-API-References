---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的标准函数名称设置区域相关的函数名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

根据给定的标准函数名称设置区域性相关函数名称。

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localfontStyleName | String | 用于页眉/页脚的区域字体样式名称。 |
| standardName | String | 标准（en-US 区域）函数名。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为工作表创建页面设置选项
            PageSetup pageSetup = worksheet.PageSetup;

            // 设置包含一些文本的页眉
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // 创建全局化设置实例
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // 调用 SetStandardHeaderFooterFontStyleName 方法
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // 将全局化设置应用于工作簿
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // 当文档被渲染或打印时，效果将可见
                // 页眉/页脚中的字体样式 "Arial" 将被视为 "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


