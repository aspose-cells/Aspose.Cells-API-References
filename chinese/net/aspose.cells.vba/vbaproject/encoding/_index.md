---
title: "VbaProject.Encoding"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "VbaProject 属性。获取和设置 VBA 项目的编码"
type: docs
url: /zh/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

获取和设置 VBA 项目的编码。

```csharp
public Encoding Encoding { get; set; }
```

### 示例

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 初始化 VBA 项目
            VbaProject vbaProject = workbook.VbaProject;

            // 设置 VBA 项目属性，包括编码
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // 向 VBA 项目添加模块
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // 保存包含 VBA 项目的工作簿
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### 另请参见

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


