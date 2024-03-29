---
title: AddIcons
second_title: Aspose.Cells for .NET API 参考
description: 添加 svg 图像
type: docs
weight: 120
url: /zh/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

添加 svg 图像。

```csharp
public Picture AddIcons(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width, byte[] imageByteData, byte[] compatibleImageData)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | Int32 | 左上行索引。 |
| top | Int32 | 表示形状与其左行的垂直偏移量，以像素为单位。 |
| upperLeftColumn | Int32 | 左上列索引。 |
| left | Int32 | 形状与其左列的水平偏移量，以像素为单位。 |
| height | Int32 | 形状的高度，以像素为单位。 |
| width | Int32 | 形状的宽度，以像素为单位。 |
| imageByteData | Byte[] | 图像字节数据。 |
| compatibleImageData | Byte[] | 从 svg 转换图像数据，以便与 Excel 2016 或更低版本兼容。 |

### 例子

```csharp

[C#]
//添加图标
using (FileStream fs = new FileStream("icon.svg", FileMode.Open))
{
    int len = (int)fs.Length;
    byte[] imageData = new byte[len];
    fs.Read(imageData, 0, len);
    Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
}
```

### 也可以看看

* class [Picture](../../picture)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
