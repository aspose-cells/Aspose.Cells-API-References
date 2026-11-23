---
title: "类 LowCodeImageSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeImageSaveOptions 类。以低代码方式保存图像的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

以低代码方式保存图像的选项。

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | 用于渲染图像的选项。 |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | 获取并设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，[`OutputStream`](../lowcodesaveoptions/outputstream/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | 获取并设置用于写入生成数据的流。当将此属性设置为非 null 时，[`OutputFile`](../lowcodesaveoptions/outputfile/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | 获取或设置保存格式。 |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | 用于保存生成图像的保存选项提供程序。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 向工作表添加示例数据
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // 创建 LowCodeImageSaveOptions 的实例
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // 设置基本属性
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // 显示当前设置
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // 修改一些图像选项
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // 创建一个简单的保存选项提供程序
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // 将工作表保存为图像
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


