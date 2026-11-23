---
title: "类 LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders 类。实现提供保存选项，以将拆分部件保存到文件，且结果文件的路径使用占位符定义"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

实现提供保存选项，以将拆分的部分保存到文件，并且生成文件的路径使用占位符定义。

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | 实例化一个对象，根据指定的模板提供保存选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | 是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引、名称及相应前缀（[`SheetNamePrefix`](./sheetnameprefix/)）不会添加到文件路径中。 |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | 是否始终在文件路径中添加拆分部件索引。默认值为 false，即当只有一个拆分部件时，拆分部件索引及相应前缀（[`SplitPartPrefix`](./splitpartprefix/)）不会添加到文件路径中。 |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | 在 [`GetSaveOptions`](./getsaveoptions/) 中创建保存选项实例的模板。 |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | 工作表索引的偏移量，即文件路径中使用的索引与实际值之间的差异（[`SheetIndex`](../splitpartinfo/sheetindex/)）。 |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | 工作表索引的前缀。 |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | 工作表索引的前缀。 |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | 拆分部件索引的偏移量，即文件路径中使用的索引与实际值之间的差异（[`PartIndex`](../splitpartinfo/partindex/)）。 |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | 拆分部件索引的前缀。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | 在处理当前拆分部件后释放资源。（继承自 [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/)。） |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | 获取用于获取当前拆分部件输出设置的保存选项。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 使用示例数据填充工作表
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // 使用包含占位符的路径模板创建提供程序
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // 配置提供程序属性
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // 配置保存选项模板
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // 为拆分渲染配置图像或打印选项
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // 创建带拆分配置的工作表渲染
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


