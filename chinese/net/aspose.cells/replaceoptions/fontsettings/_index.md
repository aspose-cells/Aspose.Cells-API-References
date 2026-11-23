---
title: "ReplaceOptions.FontSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ReplaceOptions 属性。用于被替换文本的富格式设置"
type: docs
url: /zh/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

用于被替换文本的富格式设置。

```csharp
public FontSetting[] FontSettings { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在单元格 A1 中设置示例文本
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // 使用字体设置创建替换选项
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // 为替换文本创建字体设置
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // 将字体设置应用于替换选项
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // 执行替换操作
            workbook.Replace("text", "REPLACED", options);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


