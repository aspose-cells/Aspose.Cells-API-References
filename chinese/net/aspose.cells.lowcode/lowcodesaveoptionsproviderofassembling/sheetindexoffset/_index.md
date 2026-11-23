---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 属性。文件路径中使用的工作表索引与其实际值 SheetIndex 之间的偏移量。"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

工作表索引在文件路径中使用的值与其实际值（[`SheetIndex`](../../splitpartinfo/sheetindex/)）之间的偏移量。

```csharp
public int SheetIndexOffset { get; set; }
```

### 备注

仅在 [`UseSheetName`](../usesheetname/) 为 false 时生效。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // 创建一个包含多个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // 初始化保存选项提供程序
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // 显示原始偏移量
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // 使用初始偏移量保存（工作表将编号为 10 和 11）
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // 更改偏移量并再次保存
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // 使用新偏移量保存（工作表将编号为 100 和 101）
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


