---
title: "Shape 类"
linktitle: "Shape"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Shape 类。封装在 Go 中表示 shape 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shape/
---

## Shape class

表示 msodrawing 对象。

```go

type Shape struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetMacroName](./getmacroname/) | 获取和设置宏的名称。 |
| [SetMacroName](./setmacroname/) | 获取和设置宏的名称。 |
| [IsEquation](./isequation/) | 指示形状是否仅包含公式。 |
| [IsSmartArt](./issmartart/) | 指示形状是否为智能艺术。 |
| [ToFrontOrBack](./tofrontorback/) | 将形状置于前面或发送到后面。 |
| [GetZOrderPosition](./getzorderposition/) | 返回形状在 Z 顺序中的位置。 |
| [SetZOrderPosition](./setzorderposition/) | 返回形状在 Z 顺序中的位置。 |
| [GetName](./getname/) | 获取并设置形状的名称。 |
| [SetName](./setname/) | 获取并设置形状的名称。 |
| [GetAlternativeText](./getalternativetext/) | 返回或设置 Shape 对象的描述性（替代）文本字符串。 |
| [SetAlternativeText](./setalternativetext/) | 返回或设置 Shape 对象的描述性（替代）文本字符串。 |
| [GetTitle](./gettitle/) | 指定当前形状对象的标题（说明）。 |
| [SetTitle](./settitle/) | 指定当前形状对象的标题（说明）。 |
| [GetLine](./getline/) | 获取线条样式 |
| [GetFill](./getfill/) | 返回一个 FillFormat 对象，其中包含指定形状的填充格式属性。 |
| [GetShadowEffect](./getshadoweffect/) | 表示一个 Drawing.ShadowEffect 对象，用于指定图表元素或形状的阴影效果。 |
| [GetReflection](./getreflection/) | 表示一个 ReflectionEffect 对象，用于指定图表元素或形状的反射效果。 |
| [GetGlow](./getglow/) | 表示一个 GlowEffect 对象，用于指定图表元素或形状的发光效果。 |
| [GetSoftEdges](./getsoftedges/) | 获取并设置要应用于边缘的模糊半径，单位为点。 |
| [SetSoftEdges](./setsoftedges/) | 获取并设置要应用于边缘的模糊半径，单位为点。 |
| [GetThreeDFormat](./getthreedformat/) | 获取并设置形状的 3D 格式。 |
| [GetFormatPicture](./getformatpicture/) | 获取并设置图片格式的选项。 |
| [IsHidden](./ishidden/) | 指示对象是否可见。 |
| [SetIsHidden](./setishidden/) | 指示对象是否可见。 |
| [IsAspectRatioLocked](./isaspectratiolocked/) | True 表示形状的宽高比被锁定。 |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | True 表示形状的宽高比被锁定。 |
| [GetLockedProperty](./getlockedproperty/) | 获取 locked 属性的值。 |
| [SetLockedProperty](./setlockedproperty/) | 设置 locked 属性。 |
| [GetRotationAngle](./getrotationangle/) | 获取并设置形状的旋转角度。 |
| [SetRotationAngle](./setrotationangle/) | 获取并设置形状的旋转角度。 |
| [AddHyperlink](./addhyperlink/) | 向形状添加超链接。 |
| [RemoveHyperlink](./removehyperlink/) | 移除形状的超链接。 |
| [GetHyperlink](./gethyperlink/) | 获取形状的超链接。 |
| [MoveToRange](./movetorange/) | 将形状移动到指定范围。 |
| [AlignTopRightCorner](./aligntoprightcorner/) | 将图片移动到右上角。 |
| [GetId](./getid/) | 获取此形状的标识符。 |
| [GetSpid](./getspid/) | 指定一个可选的字符串标识符，应用程序可使用它来识别特定形状。 |
| [GetSpt](./getspt/) | 指定一个可选的数字，应用程序可使用它将特定形状关联到已定义的形状类型。 |
| [GetWorksheet](./getworksheet/) | 获取包含此形状的 Aspose.Cells.Worksheet 对象。 |
| [IsGroup](./isgroup/) | 指示此形状是否为组形状。 |
| [IsInGroup](./isingroup/) | 指示该形状是否已分组。 |
| [IsWordArt](./iswordart/) | 指示此形状是否为文字艺术。 |
| [GetTextEffect](./gettexteffect/) | 返回一个 TextEffectFormat 对象，其中包含指定形状的文字效果格式属性。适用于表示 WordArt 的 Shape 对象。 |
| [IsLocked](./islocked/) | True 表示在工作表受保护时对象无法被修改。请注意，此值仅在工作表或工作表中的对象受保护时才有意义。 |
| [SetIsLocked](./setislocked/) | True 表示在工作表受保护时对象无法被修改。请注意，此值仅在工作表或工作表中的对象受保护时才有意义。 |
| [IsPrintable](./isprintable/) | 指示对象是否可打印。如果为 False，则在打印时此形状不会被打印。 |
| [SetIsPrintable](./setisprintable/) | 指示对象是否可打印。如果为 False，则在打印时此形状不会被打印。 |
| [GetMsoDrawingType](./getmsodrawingtype/) | 获取绘图类型。 |
| [GetAutoShapeType](./getautoshapetype/) | 获取并设置自动形状类型。 |
| [SetAutoShapeType](./setautoshapetype/) | 获取并设置自动形状类型。 |
| [GetAnchorType](./getanchortype/) | 获取并设置形状锚点占位符的类型。 |
| [SetAnchorType](./setanchortype/) | 获取并设置形状锚点占位符的类型。 |
| [GetPlacement](./getplacement/) | 表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置。 |
| [SetPlacement](./setplacement/) | 表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置。 |
| [GetUpperLeftRow](./getupperleftrow/) | 表示顶部行索引。 |
| [SetUpperLeftRow](./setupperleftrow/) | 表示顶部行索引。 |
| [GetUpperDeltaY](./getupperdeltay/) | 获取或设置形状相对于其左上角行的垂直偏移量。 |
| [SetUpperDeltaY](./setupperdeltay/) | 获取或设置形状相对于其左上角行的垂直偏移量。 |
| [GetUpperLeftColumn](./getupperleftcolumn/) | 表示左上角列索引。 |
| [SetUpperLeftColumn](./setupperleftcolumn/) | 表示左上角列索引。 |
| [GetUpperDeltaX](./getupperdeltax/) | 获取或设置形状相对于其左上角列的水平偏移量。 |
| [SetUpperDeltaX](./setupperdeltax/) | 获取或设置形状相对于其左上角列的水平偏移量。 |
| [GetLowerRightRow](./getlowerrightrow/) | 表示右下角行索引。 |
| [SetLowerRightRow](./setlowerrightrow/) | 表示右下角行索引。 |
| [GetLowerDeltaY](./getlowerdeltay/) | 获取或设置形状相对于其右下角行的垂直偏移量。 |
| [SetLowerDeltaY](./setlowerdeltay/) | 获取或设置形状相对于其右下角行的垂直偏移量。 |
| [GetLowerRightColumn](./getlowerrightcolumn/) | 表示右下角列索引。 |
| [SetLowerRightColumn](./setlowerrightcolumn/) | 表示右下角列索引。 |
| [GetLowerDeltaX](./getlowerdeltax/) | 获取或设置形状相对于其右下角列的水平偏移量。 |
| [SetLowerDeltaX](./setlowerdeltax/) | 获取或设置形状相对于其右下角列的水平偏移量。 |
| [GetRight](./getright/) | 表示形状相对于其右下角列的水平偏移量的宽度，单位为像素。 |
| [SetRight](./setright/) | 表示形状相对于其右下角列的水平偏移量的宽度，单位为像素。 |
| [GetBottom](./getbottom/) | 表示形状相对于其右下角行的垂直偏移量的宽度，单位为像素。 |
| [SetBottom](./setbottom/) | 表示形状相对于其右下角行的垂直偏移量的宽度，单位为像素。 |
| [GetWidth](./getwidth/) | 表示形状的宽度，单位为像素。 |
| [SetWidth](./setwidth/) | 表示形状的宽度，单位为像素。 |
| [GetWidthInch](./getwidthinch/) | 表示形状的宽度，单位为英寸。 |
| [SetWidthInch](./setwidthinch/) | 表示形状的宽度，单位为英寸。 |
| [GetWidthPt](./getwidthpt/) | 表示形状的宽度，单位为磅。 |
| [SetWidthPt](./setwidthpt/) | 表示形状的宽度，单位为磅。 |
| [GetWidthCM](./getwidthcm/) | 表示形状的宽度，单位为厘米。 |
| [SetWidthCM](./setwidthcm/) | 表示形状的宽度，单位为厘米。 |
| [GetHeight](./getheight/) | 表示形状的高度，单位为像素。 |
| [SetHeight](./setheight/) | 表示形状的高度，单位为像素。 |
| [GetHeightInch](./getheightinch/) | 表示形状的高度，单位为英寸。 |
| [SetHeightInch](./setheightinch/) | 表示形状的高度，单位为英寸。 |
| [GetHeightPt](./getheightpt/) | 表示形状的高度，单位为点。 |
| [SetHeightPt](./setheightpt/) | 表示形状的高度，单位为点。 |
| [GetHeightCM](./getheightcm/) | 表示形状的高度，单位为厘米。 |
| [SetHeightCM](./setheightcm/) | 表示形状的高度，单位为厘米。 |
| [GetLeft](./getleft/) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [SetLeft](./setleft/) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [GetLeftInch](./getleftinch/) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [SetLeftInch](./setleftinch/) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [GetLeftCM](./getleftcm/) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [SetLeftCM](./setleftcm/) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [GetTop](./gettop/) | 表示形状相对于其顶部行的垂直偏移，单位为像素。 |
| [SetTop](./settop/) | 表示形状相对于其顶部行的垂直偏移，单位为像素。 |
| [GetTopInch](./gettopinch/) | 表示形状相对于其顶部行的垂直偏移，单位为英寸。 |
| [SetTopInch](./settopinch/) | 表示形状相对于其顶部行的垂直偏移，单位为英寸。 |
| [GetTopCM](./gettopcm/) | 表示形状相对于其顶部行的垂直偏移，单位为厘米。 |
| [SetTopCM](./settopcm/) | 表示形状相对于其顶部行的垂直偏移，单位为厘米。 |
| [GetTopToCorner](./gettoptocorner/) | 获取和设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [SetTopToCorner](./settoptocorner/) | 获取和设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [GetLeftToCorner](./getlefttocorner/) | 获取和设置形状相对于工作表左边界的水平偏移。 |
| [SetLeftToCorner](./setlefttocorner/) | 获取和设置形状相对于工作表左边界的水平偏移。 |
| [GetX](./getx/) | 获取和设置形状相对于工作表左边界的水平偏移，单位为像素。 |
| [SetX](./setx/) | 获取和设置形状相对于工作表左边界的水平偏移，单位为像素。 |
| [GetY](./gety/) | 获取和设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [SetY](./sety/) | 获取和设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [GetWidthScale](./getwidthscale/) | 获取和设置宽度比例，单位为原始图片宽度的百分比。如果形状不是图片，WidthScale 属性仅返回 100； |
| [SetWidthScale](./setwidthscale/) | 获取和设置宽度比例，单位为原始图片宽度的百分比。如果形状不是图片，WidthScale 属性仅返回 100； |
| [GetHeightScale](./getheightscale/) | 获取和设置高度比例，单位为原始图片高度的百分比。如果形状不是图片，HeightScale 属性仅返回 100； |
| [SetHeightScale](./setheightscale/) | 获取和设置高度比例，单位为原始图片高度的百分比。如果形状不是图片，HeightScale 属性仅返回 100； |
| [GetTopInShape](./gettopinshape/) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [SetTopInShape](./settopinshape/) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [GetLeftInShape](./getleftinshape/) | 表示形状相对于父形状左侧边界的水平偏移，单位为父形状宽度的 1/4000。 |
| [SetLeftInShape](./setleftinshape/) | 表示形状相对于父形状左侧边界的水平偏移，单位为父形状宽度的 1/4000。 |
| [GetWidthInShape](./getwidthinshape/) | 表示形状的宽度，单位为父形状的 1/4000。 |
| [SetWidthInShape](./setwidthinshape/) | 表示形状的宽度，单位为父形状的 1/4000。 |
| [GetHeightInShape](./getheightinshape/) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [SetHeightInShape](./setheightinshape/) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [GetGroup](./getgroup/) | 获取包含此形状的组形状。 |
| [GetType](./gettype/) | 获取自动形状类型。 |
| [GetHasLine](./gethasline/) | 获取和设置形状的线条边框是否可见。 |
| [SetHasLine](./sethasline/) | 获取和设置形状的线条边框是否可见。 |
| [IsFilled](./isfilled/) | 指示填充格式是否可见。 |
| [SetIsFilled](./setisfilled/) | 指示填充格式是否可见。 |
| [IsFlippedHorizontally](./isflippedhorizontally/) | 获取和设置形状是否水平翻转。 |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | 获取和设置形状是否水平翻转。 |
| [IsFlippedVertically](./isflippedvertically/) | 获取和设置形状是否垂直翻转。 |
| [SetIsFlippedVertically](./setisflippedvertically/) | 获取和设置形状是否垂直翻转。 |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | 获取实际的底部行。 |
| [GetConnectionPoints](./getconnectionpoints/) | 获取连接点 |
| [ToImage_ImageType](./toimage_imagetype/) | 创建形状图像并以指定格式保存到流中。 |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | 将形状保存到文件。 |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | 将形状保存到流。 |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | 指示形状是否相对于原始图片大小。 |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | 指示形状是否相对于原始图片大小。 |
| [GetLinkedCell](./getlinkedcell/) | 获取或设置链接到控件值的工作表范围。 |
| [SetLinkedCell_String](./setlinkedcell_string/) | 获取或设置链接到控件值的工作表范围。 |
| [GetInputRange](./getinputrange/) | 获取或设置用于填充指定组合框的工作表范围。 |
| [SetInputRange_String](./setinputrange_string/) | 获取或设置用于填充指定组合框的工作表范围。 |
| [GetLinkedCell_Bool_Bool](./getlinkedcell_bool_bool/) | 获取与控件值关联的范围。 |
| [SetLinkedCell_String_Bool_Bool](./setlinkedcell_string_bool_bool/) | 设置与控件值关联的范围。 |
| [GetInputRange_Bool_Bool](./getinputrange_bool_bool/) | 获取用于填充控件的范围。 |
| [SetInputRange_String_Bool_Bool](./setinputrange_string_bool_bool/) | 设置用于填充控件的范围。 |
| [UpdateSelectedValue](./updateselectedvalue/) | 通过链接单元格的值更新所选值。 |
| [GetTextShapeType](./gettextshapetype/) | 获取和设置预设文本形状类型。 |
| [SetTextShapeType](./settextshapetype/) | 获取和设置预设文本形状类型。 |
| [GetTextBody](./gettextbody/) | 获取和设置形状文本的设置。 |
| [GetFont](./getfont/) | 表示形状的字体。 |
| [SetFont](./setfont/) | 表示形状的字体。 |
| [GetTextOptions](./gettextoptions/) | 表示形状的文本选项。 |
| [SetTextOptions](./settextoptions/) | 表示形状的文本选项。 |
| [CalculateTextSize](./calculatetextsize/) | 重新计算文本区域 |
| [GetText](./gettext/) | 获取和设置此形状的文本。 |
| [SetText](./settext/) | 获取和设置此形状的文本。 |
| [IsRichText](./isrichtext/) | 文本是否为富文本。 |
| [GetHtmlText](./gethtmltext/) | 获取和设置此文本框中包含数据和一些格式的 HTML 字符串。 |
| [SetHtmlText](./sethtmltext/) | 获取和设置此文本框中包含数据和一些格式的 HTML 字符串。 |
| [FormatCharacters](./formatcharacters/) | 使用字体设置格式化某些字符。 |
| [Characters](./characters/) | 返回表示文本中字符范围的 Characters 对象。 |
| [GetRichFormattings](./getrichformattings/) | 返回所有表示文本中字符范围的 Characters 对象。 |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | 获取和设置包含文本的形状的文本垂直溢出类型。 |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | 获取和设置包含文本的形状的文本垂直溢出类型。 |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | 获取和设置包含文本的形状的文本水平溢出类型。 |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | 获取和设置包含文本的形状的文本水平溢出类型。 |
| [IsTextWrapped](./istextwrapped/) | 获取和设置包含文本的形状的文本换行类型。 |
| [SetIsTextWrapped](./setistextwrapped/) | 获取和设置包含文本的形状的文本换行类型。 |
| [GetTextOrientationType](./gettextorientationtype/) | 获取和设置形状的文本方向类型。 |
| [SetTextOrientationType](./settextorientationtype/) | 获取和设置形状的文本方向类型。 |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | 获取和设置形状的文本水平对齐类型。 |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | 获取和设置形状的文本水平对齐类型。 |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | 获取和设置形状的文本垂直对齐类型。 |
| [SetTextVerticalAlignment](./settextverticalalignment/) | 获取和设置形状的文本垂直对齐类型。 |
| [GetTextDirection](./gettextdirection/) | 获取/设置此对象的文本流方向。 |
| [SetTextDirection](./settextdirection/) | 获取/设置此对象的文本流方向。 |
| [GetTextBoxOptions](./gettextboxoptions/) | 获取形状中的文本信息 |
| [GetControlData](./getcontroldata/) | 获取控件的数据。 |
| [GetActiveXControl](./getactivexcontrol/) | 获取 ActiveX 控件。 |
| [RemoveActiveXControl](./removeactivexcontrol/) | 移除 activeX 控件。 |
| [GetPaths](./getpaths/) | 获取自定义几何形状的路径。 |
| [GetGeometry](./getgeometry/) | 获取几何信息 |
| [GetCreateId](./getcreateid/) | 获取并设置此形状的创建 ID。 |
| [SetCreateId](./setcreateid/) | 获取并设置此形状的创建 ID。 |
| [IsDecorative](./isdecorative/) | 指示对象是否为装饰性。 |
| [SetIsDecorative](./setisdecorative/) | 指示对象是否为装饰性。 |
| [GetActualBox](./getactualbox/) | 获取形状的实际位置和大小（在应用旋转、翻转等之后）。 |
| [FitToTextSize](./fittotextsize/) | 重新计算适合显示所有文本内容的文本区域。 |
| [GetResultOfSmartArt](./getresultofsmartart/) | 将 SmartArt 转换为组合形状。 |
| [IsSameSetting](./issamesetting/) | 返回形状是否相同。 |
