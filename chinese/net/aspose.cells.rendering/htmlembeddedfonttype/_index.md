---
title: "枚举 HtmlEmbeddedFontType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.HtmlEmbeddedFontType 枚举。表示 HTML 中的嵌入字体类型"
type: docs
url: /zh/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

表示 HTML 中的嵌入字体类型。

```csharp
public enum HtmlEmbeddedFontType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 不嵌入字体。 |
| Woff | `1` | 嵌入 WOFF 字体。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            try
            {
                // 演示使用 HtmlEmbeddedFontType 枚举值
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // 显示枚举值
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // 演示比较
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // 显示数值
                Console.WriteLine("Numeric value for None: " + (int)noneType);
                Console.WriteLine("Numeric value for Woff: " + (int)woffType);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlEmbeddedFontType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


