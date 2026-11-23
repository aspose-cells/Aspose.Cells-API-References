---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeLoadOptionsProvider 属性。获取用于加载当前处理部分数据的加载选项"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

获取用于加载当前处理部分数据的加载选项。

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // 使用我们的加载选项初始化自定义提供程序
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // 访问 Current 属性以获取活动加载选项
                Console.WriteLine($"Processing set {counter}");
                    
                // 使用当前加载选项的输入文件/流创建工作簿
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // 演示因缺少属性而移除的选项影响
                worksheet.Cells["A1"].Value = "Sample Value";

                // 保存结果
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // 使用 IDisposable 的自定义提供程序实现
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }

            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }

    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


