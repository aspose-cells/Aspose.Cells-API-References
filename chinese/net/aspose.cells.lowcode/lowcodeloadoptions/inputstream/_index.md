---
title: "LowCodeLoadOptions.InputStream"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeLoadOptions 属性。获取和设置模板的流"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

获取并设置模板的流。

```csharp
public Stream InputStream { get; set; }
```

### 备注

当为此属性设置非 null 的流时，先前为 [`InputFile`](../inputfile/) 设置的值将被忽略。

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // 在内存流中创建示例数据
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // 使用 InputStream 创建加载选项
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // 使用流创建新的工作簿
                using (Workbook workbook = new Workbook(stream))
                {
                    // 访问第一个工作表
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // 演示内容已加载
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


