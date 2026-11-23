---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cells 方法。获取所有包含嵌入图片的单元格"
type: docs
url: /zh/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

获取所有包含嵌入图片的单元格。

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### 返回值

枚举器，用于枚举所有包含嵌入图片的 Cell 对象

### 备注

如果此工作表中没有设置为"放置在单元格" 的图片，将返回 null。

### 示例

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            
            // 向工作表添加图片（此图片不会被 GetCellsWithPlaceInCellPicture 计数）
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // 向单元格 B3 添加嵌入图像（此图像将被计数）
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // 移除浮动图片
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // 获取包含嵌入图像的单元格
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // 保存并重新加载以验证持久性
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // 重新加载后进行验证
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### 另请参见

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


