---
title: "类 AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider 类。用于为使用多个输入（如模板文件）的过程提供多种加载选项的实现"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

实现提供多种加载选项，以供使用多个输入（例如模板文件）的流程使用。

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## 属性

| 名称 | 描述 |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | 获取用于加载当前处理部分数据的加载选项。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | 在处理当前输入部分后释放资源。 |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | 检查是否还有更多输入。 |

### 备注

例如，[`SpreadsheetMerger`](../spreadsheetmerger/) 功能需要多个模板文件进行合并。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // 创建 AbstractLowCodeLoadOptionsProvider 的自定义实现
            var provider = new CustomLoadOptionsProvider();

            // 使用提供程序处理多个输入
            while (provider.MoveNext())
            {
                // 获取当前加载选项
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // 使用当前选项创建工作簿
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // 演示工作簿的使用
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // 完成此部分的处理
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // 每个部分的清理或完成逻辑
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


