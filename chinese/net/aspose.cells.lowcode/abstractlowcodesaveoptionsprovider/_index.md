---
title: "类 AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider 类。实现提供多个保存选项，以满足需要多个输出的过程。例如，SpreadsheetSplitter 功能需要多个目标来保存拆分后的文件"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

实现提供多个保存选项，以满足需要多个输出的过程。例如，[`SpreadsheetSplitter`](../spreadsheetsplitter/) 功能需要多个目标来保存拆分后的文件。

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | 在处理当前拆分部分后释放资源。 |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | 获取用于当前拆分部分的输出设置的保存选项。返回 null 表示跳过给定的部分。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // 通过扩展 AbstractLowCodeSaveOptionsProvider 创建自定义提供程序
            var customProvider = new CustomSaveOptionsProvider();

            // 创建工作簿和工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充一些数据
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // 创建拆分部分信息——在实际使用中，这将来自 API
            // 由于无法直接构造它，这里仅传入 null 进行演示
            SplitPartInfo splitPartInfo = null;
            
            // 从提供程序获取保存选项
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // 配置保存选项（示例）
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // 演示完成该过程
            customProvider.Finish(saveOptions);
            
            // 保存工作簿（与提供程序无直接关系，仅作演示）
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // AbstractLowCodeSaveOptionsProvider 的自定义实现
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // 基于部分信息创建并返回自定义保存选项
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // 已移除 CachedFileFolder，因为它在 LowCodeSaveOptions 中不存在
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // 此处进行清理或结束逻辑
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


