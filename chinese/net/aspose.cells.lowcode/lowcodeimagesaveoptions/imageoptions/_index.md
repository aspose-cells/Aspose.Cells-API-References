---
title: "LowCodeImageSaveOptions.ImageOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeImageSaveOptions 属性。用于渲染图像的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/
---
## LowCodeImageSaveOptions.ImageOptions property

用于渲染图像的选项。

```csharp
public ImageOrPrintOptions ImageOptions { get; set; }
```

### 备注

当指定一个 [`ImageOrPrintOptions`](../../../aspose.cells.rendering/imageorprintoptions/) 实例时，[`SaveFormat`](../saveformat/) 将被覆盖（如果之前已指定）。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Output");

            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.ImageOptions = new ImageOrPrintOptions();

            Console.WriteLine("Default Horizontal Resolution: " + saveOptions.ImageOptions.HorizontalResolution);
            
            saveOptions.ImageOptions.HorizontalResolution = 300;
            saveOptions.ImageOptions.VerticalResolution = 300;
            SheetRender highResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            highResRenderer.ToImage(0, "HighResolutionOutput.png");

            saveOptions.ImageOptions.HorizontalResolution = 150;
            saveOptions.ImageOptions.VerticalResolution = 150;
            SheetRender lowResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            lowResRenderer.ToImage(0, "LowResolutionOutput.png");
        }
    }
}
```

### 另请参见

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


