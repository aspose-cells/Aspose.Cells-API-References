---
title: "LowCodeMergeOptions.SaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeMergeOptions 属性。用于保存拆分部分的保存选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodemergeoptions/saveoptions/
---
## LowCodeMergeOptions.SaveOptions property

用于保存拆分后部分的保存选项。

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Merged Data");

            // 初始化合并选项
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));

            // 配置新的保存选项
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            // 通过工作簿设置设置密码
            workbook.Settings.Password = "Aspose1234!";
            mergeOptions.SaveOptions = saveOptions;

            // 通过使用配置的选项保存来演示效果
            workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Workbook saved with password-protected SaveOptions.");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


