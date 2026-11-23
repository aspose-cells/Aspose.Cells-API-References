---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeMergeOptions 属性。用于保存拆分部分的保存选项提供程序"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

提供用于保存拆分后部分的保存选项的提供程序。

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### 备注

如果指定此属性，[`LoadOptions`](../../../aspose.cells/loadoptions/) 将不起作用，因为每个拆分部分的输出将由提供程序指定。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 LowCodeMergeOptions 的实例
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // 显示 LoadOptionsProvider 的当前值（初始应为 null）
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // 创建自定义 LoadOptionsProvider 实现
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // 演示设置该属性
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // 使用带有提供程序的合并选项
            // 这通常会与处理多个文件的方法一起使用
            // 为了演示，我们只检查提供程序是否可以移动到下一个
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // 保存工作簿
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // 模拟有 3 个文件需要处理
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // 此处应放置清理或结束逻辑
            }
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


