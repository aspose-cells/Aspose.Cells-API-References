---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ConditionalFormattingIcon 方法。获取具有单元格设置的图像数据"
type: docs
url: /zh/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

获取具有单元格设置的图像数据。

```csharp
public byte[] GetImageData(Cell cell)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 单元格 | 单元格 | 单元格的设置。 |

### 返回值

返回图标的图像数据。

### 示例

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### 另请参见

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


