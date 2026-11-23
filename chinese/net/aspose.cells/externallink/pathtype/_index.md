---
title: "ExternalLink.PathType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalLink 属性。获取此外部链接的路径类型"
type: docs
url: /zh/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

获取此外部链接的路径类型

```csharp
public string PathType { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表
            Worksheet sheet = workbook.Worksheets[0];
            
            // 创建指向另一本工作簿的外部链接
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // 获取外部链接
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // 显示外部链接的路径类型
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // 保存工作簿
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


