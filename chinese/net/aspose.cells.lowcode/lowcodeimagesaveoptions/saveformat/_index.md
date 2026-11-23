---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeImageSaveOptions 属性。获取或设置保存格式"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

获取或设置保存格式。

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### 备注

如果已指定 [`ImageOptions`](../imageoptions/)，设置此属性还会更改其 [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) 的值。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // 使用默认值初始化 LowCodeImageSaveOptions
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // 显示初始 SaveFormat（默认是 Png）
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // 配置为 JPEG 输出
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // 更改为 PNG 格式并再次保存
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // 使用配置的选项渲染工作表
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### 另请参见

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


