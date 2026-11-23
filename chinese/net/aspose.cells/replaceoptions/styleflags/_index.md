---
title: "ReplaceOptions.StyleFlags"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ReplaceOptions 属性。获取并设置应用字体设置的标志"
type: docs
url: /zh/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

获取并设置应用字体设置的标志。

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向单元格添加示例文本
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // 创建替换选项
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // 创建字体设置和样式标志
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // 配置字体和样式
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // 将设置应用于选项
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // 执行替换
            workbook.Replace("test", replacementText, options);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


