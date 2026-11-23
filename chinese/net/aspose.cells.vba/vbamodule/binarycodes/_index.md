---
title: "VbaModule.BinaryCodes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "VbaModule 属性。获取和设置模块的二进制代码"
type: docs
url: /zh/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

获取和设置模块的二进制代码。

```csharp
public byte[] BinaryCodes { get; }
```

### 示例

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // 加载带有 VBA 项目的工作簿
            Workbook workbook = new Workbook("example.xlsm");
            
            // 访问 VBA 项目
            VbaProject vbaProject = workbook.VbaProject;
            
            // 从第一个模块获取二进制代码
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // 使用中文编码 (936) 将其转换为字符串
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // 输出包含中文字符的内容
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### 另请参见

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


