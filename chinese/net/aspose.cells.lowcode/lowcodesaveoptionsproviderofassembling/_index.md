---
title: "类 LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling 类。实现提供保存选项，以将拆分部分保存到文件，并且生成文件的路径命名方式可能包含目录：PathHeader SheetPrefix SheetIndex 或 SheetName SplitPartPrefix SplitPartIndex PathTail"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

实现提供保存选项，以将拆分部分保存到文件，并且生成文件的路径命名方式为（可能包含目录）：[`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex（或 SheetName）+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/)。

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | 是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀不会添加到文件路径中。 |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | 是否始终在文件路径中添加拆分部分索引。默认值为 false，即当只有一个拆分部分时，拆分部分索引及相应前缀不会添加到文件路径中。 |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | 文件路径的头部部分（在工作表和拆分部分内容之前）。 |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | 文件路径的尾部部分（在序列号之后）。应包含文件名的扩展名。 |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | 在 [`GetSaveOptions`](./getsaveoptions/) 中创建保存选项实例的模板。 |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | 工作表索引的偏移量，即文件路径中使用的索引与实际值之间的差异（[`SheetIndex`](../splitpartinfo/sheetindex/)）。 |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | 工作表索引的前缀。 |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | 拆分部件索引的偏移量，即文件路径中使用的索引与实际值之间的差异（[`PartIndex`](../splitpartinfo/partindex/)）。 |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | 拆分部件索引的前缀。 |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | 是否使用工作表名称而非工作表索引构建文件路径。默认值为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | 在处理当前拆分部件后释放资源。（继承自 [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/)。） |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | 获取用于获取当前拆分部件输出设置的保存选项。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // 初始化并配置保存选项提供程序
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // 使用 LowCodeSaveOptions 配置带拆分的 XLSX 保存选项
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // 使用正确的保存格式，利用提供程序启用的选项保存工作簿
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


