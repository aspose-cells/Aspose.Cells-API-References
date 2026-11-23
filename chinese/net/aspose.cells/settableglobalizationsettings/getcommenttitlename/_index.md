---
title: "SettableGlobalizationSettings.GetCommentTitleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据评论标题类型获取区域设置相关的评论标题名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getcommenttitlename/
---
## SettableGlobalizationSettings.GetCommentTitleName method

根据评论标题类型获取区域设置相关的评论标题名称。

```csharp
public override string GetCommentTitleName(CommentTitleType type)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | CommentTitleType | 评论标题的类型 |

### 返回值

区域设置相关的评论标题名称

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 在单元格 A1 中创建批注
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            comment.IsVisible = true;

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 为不同类型设置自定义评论标题名称
            settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
            settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
            settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
            settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

            // 将全局化设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 获取并显示评论标题名称
                Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
                Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
                Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
                Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("CommentTitleNamesDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


