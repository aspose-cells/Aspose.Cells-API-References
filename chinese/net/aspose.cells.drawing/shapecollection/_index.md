---
title: ShapeCollection
second_title: Aspose.Cells for .NET API 参考
description: 表示工作表/图表中的所有形状
type: docs
weight: 2650
url: /zh/net/aspose.cells.drawing/shapecollection/
---
## ShapeCollection class

表示工作表/图表中的所有形状。

```csharp
public class ShapeCollection : CollectionBase<Shape>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.drawing/shapecollection/item) { get; } | 获取特定索引处的形状对象。 (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddActiveXControl](../../aspose.cells.drawing/shapecollection/addactivexcontrol)(ControlType, int, int, int, int, int, int) | 创建一个 Activex 控件。 |
| [AddArc](../../aspose.cells.drawing/shapecollection/addarc)(int, int, int, int, int, int) | 将 ArcShape 添加到工作表。 |
| [AddAutoShape](../../aspose.cells.drawing/shapecollection/addautoshape)(AutoShapeType, int, int, int, int, int, int) | 将自选图形添加到工作表。 |
| [AddAutoShapeInChart](../../aspose.cells.drawing/shapecollection/addautoshapeinchart)(AutoShapeType, int, int, int, int) | 将自选图形添加到图表中。 |
| [AddButton](../../aspose.cells.drawing/shapecollection/addbutton)(int, int, int, int, int, int) | 向工作表添加一个按钮。 |
| [AddCheckBox](../../aspose.cells.drawing/shapecollection/addcheckbox)(int, int, int, int, int, int) | 在工作表中添加一个复选框。 |
| [AddComboBox](../../aspose.cells.drawing/shapecollection/addcombobox)(int, int, int, int, int, int) | 将 ComboBox 添加到工作表中。 |
| [AddCopy](../../aspose.cells.drawing/shapecollection/addcopy)(Shape, int, int, int, int) | 将形状添加并复制到工作表中。 |
| [AddFreeFloatingShape](../../aspose.cells.drawing/shapecollection/addfreefloatingshape)(MsoDrawingType, int, int, int, int, byte[], bool) | 向工作表添加自由浮动形状。仅适用于线条/图像形状。 |
| [AddGroupBox](../../aspose.cells.drawing/shapecollection/addgroupbox)(int, int, int, int, int, int) | 将 GroupBox 添加到工作表中。 |
| [AddIcons](../../aspose.cells.drawing/shapecollection/addicons)(int, int, int, int, int, int, byte[], byte[]) | 添加 svg 图像。 |
| [AddLabel](../../aspose.cells.drawing/shapecollection/addlabel)(int, int, int, int, int, int) | 向工作表添加标签。 |
| [AddLabelInChart](../../aspose.cells.drawing/shapecollection/addlabelinchart)(int, int, int, int) | 向图表添加标签。 |
| [AddLine](../../aspose.cells.drawing/shapecollection/addline)(int, int, int, int, int, int) | 将 LineShape 添加到工作表中。 |
| [AddLinkedPicture](../../aspose.cells.drawing/shapecollection/addlinkedpicture)(int, int, int, int, string) | 添加链接图片。 |
| [AddListBox](../../aspose.cells.drawing/shapecollection/addlistbox)(int, int, int, int, int, int) | 将列表框添加到工作表中。 |
| [AddOleObject](../../aspose.cells.drawing/shapecollection/addoleobject)(int, int, int, int, int, int, byte[]) |  |
| [AddOleObjectWithLinkedImage](../../aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage)(int, int, int, int, string) | 添加链接图片。 |
| [AddOval](../../aspose.cells.drawing/shapecollection/addoval)(int, int, int, int, int, int) | 在工作表中添加一个椭圆形。 |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture)(int, int, int, int, Stream) | 将图片添加到集合中。 |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture_1)(int, int, Stream, int, int) | 将图片添加到集合中。 |
| [AddPictureInChart](../../aspose.cells.drawing/shapecollection/addpictureinchart)(int, int, Stream, int, int) | 将图片添加到图表中。 |
| [AddRadioButton](../../aspose.cells.drawing/shapecollection/addradiobutton)(int, int, int, int, int, int) | 将 RadioButton 添加到工作表中。 |
| [AddRectangle](../../aspose.cells.drawing/shapecollection/addrectangle)(int, int, int, int, int, int) | 将 RectangleShape 添加到工作表。 |
| [AddScrollBar](../../aspose.cells.drawing/shapecollection/addscrollbar)(int, int, int, int, int, int) | 将滚动条添加到工作表。 |
| [AddShape](../../aspose.cells.drawing/shapecollection/addshape)(MsoDrawingType, int, int, int, int, int, int) | 将形状添加到工作表。 |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart)(MsoDrawingType, PlacementType, int, int, int, int) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart_1)(MsoDrawingType, PlacementType, int, int, int, int, byte[]) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale)(MsoDrawingType, PlacementType, double, double, double, double) | 向图表添加形状。所有单位都是图表区域的百分比比例。 |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale_1)(MsoDrawingType, PlacementType, double, double, double, double, byte[]) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [AddSpinner](../../aspose.cells.drawing/shapecollection/addspinner)(int, int, int, int, int, int) | 将微调器添加到工作表。 |
| [AddSvg](../../aspose.cells.drawing/shapecollection/addsvg)(int, int, int, int, int, int, byte[], byte[]) | 添加 svg 图像。 |
| [AddTextBox](../../aspose.cells.drawing/shapecollection/addtextbox)(int, int, int, int, int, int) | 在工作表中添加一个文本框。 |
| [AddTextBoxInChart](../../aspose.cells.drawing/shapecollection/addtextboxinchart)(int, int, int, int) | 向图表添加一个文本框。 |
| [AddTextEffect](../../aspose.cells.drawing/shapecollection/addtexteffect)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int, int, int) | 插入艺术字对象。 |
| [AddTextEffectInChart](../../aspose.cells.drawing/shapecollection/addtexteffectinchart)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int) | 将艺术字对象插入图表 |
| [AddWordArt](../../aspose.cells.drawing/shapecollection/addwordart)(PresetWordArtStyle, string, int, int, int, int, int, int) | 自 Excel 2007.s 添加预设艺术字 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape, IComparer&lt;Shape&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Shape, IComparer&lt;Shape&gt;) |  |
| [Clear](../../aspose.cells.drawing/shapecollection/clear#clear)() | 清除所有形状。 (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Shape) |  |
| [CopyCommentsInRange](../../aspose.cells.drawing/shapecollection/copycommentsinrange)(ShapeCollection, CellArea, int, int) | 复制范围内的所有评论。 |
| [CopyInRange](../../aspose.cells.drawing/shapecollection/copyinrange)(ShapeCollection, CellArea, int, int, bool) | 将范围内的形状复制到目标范围。 |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Shape[], int, int) |  |
| [DeleteInRange](../../aspose.cells.drawing/shapecollection/deleteinrange)(CellArea) | 删除范围内的形状。注释形状不会被删除。 |
| [DeleteShape](../../aspose.cells.drawing/shapecollection/deleteshape)(Shape) | 删除一个形状。如果形状在组中或者是评论形状，则不会被删除。 |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Shape&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Shape&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Shape&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Shape&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [Group](../../aspose.cells.drawing/shapecollection/group)(Shape[]) | 对形状进行分组。 |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int, int) |  |
| [Remove](../../aspose.cells.drawing/shapecollection/remove)(Shape) | 移除形状。 |
| [RemoveAt](../../aspose.cells.drawing/shapecollection/removeat#removeat)(int) | 移除形状。 (2 methods) |
| [Ungroup](../../aspose.cells.drawing/shapecollection/ungroup)(GroupShape) | 取消组合形状项目。 |
| [UpdateSelectedValue](../../aspose.cells.drawing/shapecollection/updateselectedvalue)() | 通过形状的链接单元格的值更新所选值。 |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();

//获取形状集合
ShapeCollection shapes = workbook.Worksheets[0].Shapes;

//做你的事

//保存excel文件。
workbook.Save("result.xlsx");
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Shape](../shape)
* 命名空间 [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
