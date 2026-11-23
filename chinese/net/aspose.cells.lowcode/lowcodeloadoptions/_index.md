---
title: "类 LowCodeLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeLoadOptions 类。用于加载模板文件的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

加载模板文件的选项。

```csharp
public class LowCodeLoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | 获取并设置模板的文件（如有需要包括路径）。 |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | 获取并设置模板的流。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // 创建示例流（内存中用于演示目的）
            using (MemoryStream stream = new MemoryStream())
            {
                // 创建新工作簿并保存到流以进行演示
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // 重置流位置
                stream.Position = 0;

                // 创建并使用 LowCodeLoadOptions
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // 示例用法 - 通常会传递给处理方法
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


