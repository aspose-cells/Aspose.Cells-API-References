---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。通过使用 CSS 自定义属性来优化 html 的输出。例如，在一个 base64 图像出现多次且使用自定义属性的情况下，图像数据只需保存一次，从而提升生成的 html 的性能。默认值为 false。"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

通过使用 CSS 自定义属性来优化 html 的输出。例如，在一个 base64 图像出现多次且使用自定义属性的情况下，图像数据只需保存一次，从而提升生成的 html 的性能。默认值为 false。

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加带格式的示例数据。
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // 添加将在多个单元格中重复的图像。
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // 将图像复制到其他位置。
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // 创建 HtmlSaveOptions 实例
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // 显示当前值。
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // 设置为 true 以优化 CSS 输出。
            htmlOptions.EnableCssCustomProperties = true;

            // 使用 CSS 优化进行保存。
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // 设置为 false 进行比较。
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


