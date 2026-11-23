---
title: "PictureCollection.Camera"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PictureCollection 方法。对范围拍照"
type: docs
url: /zh/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

对范围拍照。

```csharp
public int Camera(int row, int column, string range)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 此图片的行索引。 |
| 列 | Int32 | 此图片的列索引。 |
| 范围 | String | 需要拍照的区域 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据以创建范围
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // 从工作表获取 Pictures 集合
                PictureCollection pictures = worksheet.Pictures;

                // 调用 Camera 方法创建相机图片
                // 参数：row（左上行），column（左上列），range（源范围）
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // 保存工作簿
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


