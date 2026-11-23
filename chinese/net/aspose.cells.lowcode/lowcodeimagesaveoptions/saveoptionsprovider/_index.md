---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeImageSaveOptions 属性。用于保存生成图像的保存选项提供程序"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

用于保存生成图像的保存选项提供程序。

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### 备注

当指定此属性时，此实例指定的输出（[`OutputFile`](../../lowcodesaveoptions/outputfile/) 或 [`OutputStream`](../../lowcodesaveoptions/outputstream/)）将不生效。相反，每个生成图像的输出将由提供程序指定。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // 创建 LowCodeImageSaveOptions 实例
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // 创建自定义 SaveOptionsProvider
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // 显示当前 SaveOptionsProvider
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // 通过使用不同选项保存来演示效果
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // 更改为 null 提供程序
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // 为每个部分返回自定义保存选项
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // 在保存后执行任何清理工作
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


