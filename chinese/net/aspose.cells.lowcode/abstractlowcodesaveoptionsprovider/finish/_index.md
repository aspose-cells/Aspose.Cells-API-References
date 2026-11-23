---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeSaveOptionsProvider 方法。处理当前拆分部分后释放资源"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

在处理当前拆分部分后释放资源。

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 部分 | LowCodeSaveOptions | 用于当前拆分部分的保存选项。 |

### 备注

默认情况下，此方法仅直接关闭由 [`OutputStream`](../../lowcodesaveoptions/outputstream/) 指定的流（如果保存选项将流指定为目标）。用户可以覆盖此方法，以根据其需求以及 [`GetSaveOptions`](../getsaveoptions/) 的实现来控制资源的释放方式。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // 创建具体的提供程序实例
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // AbstractLowCodeSaveOptionsProvider 的具体实现
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // 实现所需的抽象方法
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


