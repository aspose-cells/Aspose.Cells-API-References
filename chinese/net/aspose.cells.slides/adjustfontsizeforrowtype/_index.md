---
title: "枚举 AdjustFontSizeForRowType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType 枚举。表示应调整哪种行"
type: docs
url: /zh/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

表示应调整哪种行。

```csharp
public enum AdjustFontSizeForRowType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 不调整。 |
| EmptyRows | `1` | 如果行为空，则更改字体大小以适应行高。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表填入一些数据
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // 创建一个 PptxSaveOptions 实例，并设置 AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // 将工作簿保存为 PPTX 文件
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


