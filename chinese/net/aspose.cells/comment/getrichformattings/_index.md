---
title: "Comment.GetRichFormattings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Comment 方法。返回表示评论文本中字符范围的所有 Characters 对象"
type: docs
url: /zh/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

返回表示评论文本中字符范围的所有 Characters 对象。

```csharp
public FontSetting[] GetRichFormattings()
```

### 返回值

所有 Characters 对象

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向单元格 A1 添加注释
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // 获取富文本格式
            FontSetting[] formattings = comment.GetRichFormattings();

            // 显示格式信息
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### 另请参见

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


