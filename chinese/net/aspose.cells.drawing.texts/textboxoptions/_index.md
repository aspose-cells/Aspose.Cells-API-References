---
title: "类 TextBoxOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions 类。表示形状的文本选项"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

表示形状的文本选项

```csharp
public class TextBoxOptions
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | 是否允许文本溢出形状。 |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | 返回以点为单位的底部边距 |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | 获取和设置以点为单位的左侧边距。 |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | 指示是否调整形状大小以适应文本 |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | 获取和设置以点为单位的右侧边距。 |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | 获取或设置给定文本主体内的文本显示方向。它对应 Excel 中的“格式形状 - 文本选项 - 文本框 - 文本方向”。 |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | 它对应 Excel 中的“格式形状 - 文本选项 - 文本框 - 垂直对齐”。 |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | 获取和设置以点为单位的顶部边距。 |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | 指定形状内的文本换行。False - 文本主体不会换行。True - 文本主体会换行。 |

### 示例

```csharp

[C#]
//实例化 Workbook 对象
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//执行你的业务

//保存 Excel 文件。
workbook.Save("exmaple.xlsx");
```

### 另请参见

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


