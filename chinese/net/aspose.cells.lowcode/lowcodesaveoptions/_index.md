---
title: "类 LowCodeSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeSaveOptions 类。以低代码方式保存生成结果的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

以低代码方式保存生成结果的选项。

```csharp
public class LowCodeSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | 获取并设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，[`OutputStream`](./outputstream/) 将被忽略。 |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | 获取并设置用于写入生成数据的流。当将此属性设置为非 null 时，[`OutputFile`](./outputfile/) 将被忽略。 |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | 获取并设置输出的保存格式。通常，对于低代码方式的特定处理，只允许使用某些特定格式。请为相应的处理指定正确的格式，否则可能导致意外结果甚至异常。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表并放入一些数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // 创建保存选项
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // 使用指定的选项保存工作簿
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


