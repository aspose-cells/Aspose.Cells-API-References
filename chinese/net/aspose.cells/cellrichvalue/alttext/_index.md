---
title: "CellRichValue.AltText"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellRichValue 属性。获取与图像关联的替代文本"
type: docs
url: /zh/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

获取与图像关联的替代文本。

```csharp
public virtual string AltText { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyAltTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["C4"];
            
            cell.GetRichValue().AltText = "test alt text";
            
            Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
        }
    }
}
```

### 另请参见

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


