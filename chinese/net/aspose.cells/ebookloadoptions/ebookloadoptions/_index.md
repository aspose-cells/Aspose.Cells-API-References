---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EbookLoadOptions 构造函数。创建用于加载电子书文件的选项"
type: docs
url: /zh/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

创建用于加载电子书文件的选项。

```csharp
public EbookLoadOptions()
```

### 示例

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // 使用构造函数创建 EbookLoadOptions 的实例
            EbookLoadOptions options = new EbookLoadOptions();

            // 设置一些基本属性
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // 使用指定的选项加载电子书文件
            Workbook workbook = new Workbook("sample.epub", options);
            
            // 另存为 Excel 文件
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

创建加载电子书文件的选项。

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadFormat | LoadFormat | 加载格式 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // 使用 LoadFormat 参数创建 EbookLoadOptions 实例
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // 显示确认
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // 示例用法：使用这些选项加载工作簿
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // 保存结果
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


