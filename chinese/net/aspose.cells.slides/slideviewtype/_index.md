---
title: "枚举 SlideViewType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Slides.SlideViewType 枚举。表示导出为幻灯片时的类型"
type: docs
url: /zh/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

表示导出为幻灯片时的类型。

```csharp
public enum SlideViewType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| View | `0` | 在 MS Excel 中导出为视图。 |
| Print | `1` | 导出为打印。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // 使用 SlideViewType 配置 PPTX 保存选项
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // 另存为 PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


