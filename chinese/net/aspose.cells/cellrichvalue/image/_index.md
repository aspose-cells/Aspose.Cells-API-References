---
title: "CellRichValue.Image"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellRichValue 属性。获取单元格的图像数据"
type: docs
url: /zh/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

获取单元格的图像数据。

```csharp
public virtual byte[] Image { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加图像
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // 获取包含图像的单元格富值
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // 访问富值
            CellRichValue richValue = cell.GetRichValue();

            // 显示图像属性
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // 为图像设置新的替代文本
            richValue.AltText = "Sample product image";

            // 保存工作簿
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


