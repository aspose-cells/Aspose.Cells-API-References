---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapeCollection 方法。使用 LaTeX 格式字符串向工作表添加方程对象"
type: docs
url: /zh/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

使用 LaTeX 格式字符串向工作表添加方程对象。

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | Int32 | 顶部行索引。 |
| 顶部 | Int32 | 其顶部行的垂直偏移量，单位为像素。 |
| leftColumn | Int32 | 左列索引。 |
| 左 | Int32 | 水平偏移量相对于其左列，单位为像素。 |
| height | Int32 | 公式的高度，单位为像素。 |
| 宽度 | Int32 | 公式的宽度，单位为像素。 |
| latex | String | LaTeX 格式字符串 |

### 示例

```csharp

[C#]
// LaTeX 格式字符串。
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// 向工作表添加一个公式对象。
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### 另请参见

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


