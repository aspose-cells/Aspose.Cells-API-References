---
title: "ImageOrPrintOptions.CustomRenderSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageOrPrintOptions 属性。获取或设置渲染期间的自定义设置"
type: docs
url: /zh/net/aspose.cells.rendering/imageorprintoptions/customrendersettings/
---
## ImageOrPrintOptions.CustomRenderSettings property

获取或设置渲染期间的自定义设置。

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class ImageOrPrintOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // 创建一个包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo for CustomRenderSettings");
            sheet.Cells["B2"].PutValue(12345);
            sheet.Cells["C3"].PutValue(DateTime.Now);

            try
            {
                // 初始化 ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // 访问 CustomRenderSettings 属性（只读）并显示其当前状态
                var customRenderSettings = options.CustomRenderSettings;
                Console.WriteLine("CustomRenderSettings instance: " +
                                  (customRenderSettings != null ? customRenderSettings.GetType().FullName : "null"));

                // 可选地演示这些选项仍然适用于渲染
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                SheetRender renderer = new SheetRender(sheet, options);
                renderer.ToImage(0, "CustomRenderSettingsDemo.png");

                Console.WriteLine("Image rendered successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CustomRenderSettings](../../customrendersettings/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


