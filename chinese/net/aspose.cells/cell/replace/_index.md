---
title: "Cell.Replace"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。使用选项替换单元格的文本"
type: docs
url: /zh/net/aspose.cells/cell/replace/
---
## Cell.Replace method

使用选项替换单元格的文本。

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| placeHolder | String | Cell 占位符 |
| newValue | String | 要替换的字符串值 |
| options | ReplaceOptions | 替换选项 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // 创建替换选项
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // 从单元格 B1 获取字体设置以应用于替换
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // 使用选项将所有 "hello" 的变体替换为 "Hi"
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // 保存工作簿
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


