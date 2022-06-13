---
title: ShapeCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет все фигуры на листе/диаграмме.
type: docs
weight: 2650
url: /ru/net/aspose.cells.drawing/shapecollection/
---
## ShapeCollection class

Представляет все фигуры на листе/диаграмме.

```csharp
public class ShapeCollection : CollectionBase<Shape>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.drawing/shapecollection/item) { get; } | Получает объект формы по указанному индексу. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [AddActiveXControl](../../aspose.cells.drawing/shapecollection/addactivexcontrol)(ControlType, int, int, int, int, int, int) | Создает элемент управления Activex. |
| [AddArc](../../aspose.cells.drawing/shapecollection/addarc)(int, int, int, int, int, int) | Добавляет ArcShape на рабочий лист. |
| [AddAutoShape](../../aspose.cells.drawing/shapecollection/addautoshape)(AutoShapeType, int, int, int, int, int, int) | Добавляет автофигуру на рабочий лист. |
| [AddAutoShapeInChart](../../aspose.cells.drawing/shapecollection/addautoshapeinchart)(AutoShapeType, int, int, int, int) | Добавляет автофигуру на диаграмму. |
| [AddButton](../../aspose.cells.drawing/shapecollection/addbutton)(int, int, int, int, int, int) | Добавляет кнопку на рабочий лист. |
| [AddCheckBox](../../aspose.cells.drawing/shapecollection/addcheckbox)(int, int, int, int, int, int) | Добавляет флажок на рабочий лист. |
| [AddComboBox](../../aspose.cells.drawing/shapecollection/addcombobox)(int, int, int, int, int, int) | Добавляет поле со списком на рабочий лист. |
| [AddCopy](../../aspose.cells.drawing/shapecollection/addcopy)(Shape, int, int, int, int) | Добавляет и копирует фигуру на рабочий лист. |
| [AddFreeFloatingShape](../../aspose.cells.drawing/shapecollection/addfreefloatingshape)(MsoDrawingType, int, int, int, int, byte[], bool) | Добавляет свободно плавающую фигуру на рабочий лист. Применяется только для формы линии/изображения. |
| [AddGroupBox](../../aspose.cells.drawing/shapecollection/addgroupbox)(int, int, int, int, int, int) | Добавляет GroupBox на рабочий лист. |
| [AddIcons](../../aspose.cells.drawing/shapecollection/addicons)(int, int, int, int, int, int, byte[], byte[]) | Добавляет изображение svg. |
| [AddLabel](../../aspose.cells.drawing/shapecollection/addlabel)(int, int, int, int, int, int) | Добавляет метку к рабочему листу. |
| [AddLabelInChart](../../aspose.cells.drawing/shapecollection/addlabelinchart)(int, int, int, int) | Добавляет метку к диаграмме. |
| [AddLine](../../aspose.cells.drawing/shapecollection/addline)(int, int, int, int, int, int) | Добавляет LineShape на рабочий лист. |
| [AddLinkedPicture](../../aspose.cells.drawing/shapecollection/addlinkedpicture)(int, int, int, int, string) | Добавить связанное изображение. |
| [AddListBox](../../aspose.cells.drawing/shapecollection/addlistbox)(int, int, int, int, int, int) | Добавляет ListBox на рабочий лист. |
| [AddOleObject](../../aspose.cells.drawing/shapecollection/addoleobject)(int, int, int, int, int, int, byte[]) |  |
| [AddOleObjectWithLinkedImage](../../aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage)(int, int, int, int, string) | Добавить связанное изображение. |
| [AddOval](../../aspose.cells.drawing/shapecollection/addoval)(int, int, int, int, int, int) | Добавляет овал на рабочий лист. |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture)(int, int, int, int, Stream) | Добавляет картинку в коллекцию. |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture_1)(int, int, Stream, int, int) | Добавляет картинку в коллекцию. |
| [AddPictureInChart](../../aspose.cells.drawing/shapecollection/addpictureinchart)(int, int, Stream, int, int) | Добавляет картинку на график. |
| [AddRadioButton](../../aspose.cells.drawing/shapecollection/addradiobutton)(int, int, int, int, int, int) | Добавляет RadioButton на рабочий лист. |
| [AddRectangle](../../aspose.cells.drawing/shapecollection/addrectangle)(int, int, int, int, int, int) | Добавляет RectangleShape на рабочий лист. |
| [AddScrollBar](../../aspose.cells.drawing/shapecollection/addscrollbar)(int, int, int, int, int, int) | Добавляет полосу прокрутки на рабочий лист. |
| [AddShape](../../aspose.cells.drawing/shapecollection/addshape)(MsoDrawingType, int, int, int, int, int, int) | Добавляет фигуру на рабочий лист. |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart)(MsoDrawingType, PlacementType, int, int, int, int) | Добавить фигуру на диаграмму. Все единицы измерения составляют 1/4000 области диаграммы. |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart_1)(MsoDrawingType, PlacementType, int, int, int, int, byte[]) | Добавить фигуру на диаграмму. Все единицы измерения составляют 1/4000 области диаграммы. |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale)(MsoDrawingType, PlacementType, double, double, double, double) | Добавить фигуру на диаграмму. Все единицы измерения представляют собой процентную шкалу области диаграммы. |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale_1)(MsoDrawingType, PlacementType, double, double, double, double, byte[]) | Добавить фигуру на диаграмму. Все единицы измерения составляют 1/4000 области диаграммы. |
| [AddSpinner](../../aspose.cells.drawing/shapecollection/addspinner)(int, int, int, int, int, int) | Добавляет счетчик на рабочий лист. |
| [AddSvg](../../aspose.cells.drawing/shapecollection/addsvg)(int, int, int, int, int, int, byte[], byte[]) | Добавляет изображение svg. |
| [AddTextBox](../../aspose.cells.drawing/shapecollection/addtextbox)(int, int, int, int, int, int) | Добавляет текстовое поле на рабочий лист. |
| [AddTextBoxInChart](../../aspose.cells.drawing/shapecollection/addtextboxinchart)(int, int, int, int) | Добавляет текстовое поле на график. |
| [AddTextEffect](../../aspose.cells.drawing/shapecollection/addtexteffect)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int, int, int) | Вставляет объект WordArt. |
| [AddTextEffectInChart](../../aspose.cells.drawing/shapecollection/addtexteffectinchart)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int) | Вставляет объект WordArt в диаграмму |
| [AddWordArt](../../aspose.cells.drawing/shapecollection/addwordart)(PresetWordArtStyle, string, int, int, int, int, int, int) | Добавляет предустановку WordArt начиная с Excel 2007.s |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape, IComparer&lt;Shape&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Shape, IComparer&lt;Shape&gt;) |  |
| [Clear](../../aspose.cells.drawing/shapecollection/clear#clear)() | Очистить все фигуры. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Shape) |  |
| [CopyCommentsInRange](../../aspose.cells.drawing/shapecollection/copycommentsinrange)(ShapeCollection, CellArea, int, int) | Скопировать все комментарии в диапазоне. |
| [CopyInRange](../../aspose.cells.drawing/shapecollection/copyinrange)(ShapeCollection, CellArea, int, int, bool) | Скопируйте фигуры из диапазона в целевой диапазон. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Shape[], int, int) |  |
| [DeleteInRange](../../aspose.cells.drawing/shapecollection/deleteinrange)(CellArea) | Удалить фигуры в диапазоне. Фигуры комментариев не будут удалены. |
| [DeleteShape](../../aspose.cells.drawing/shapecollection/deleteshape)(Shape) | Удалить фигуру. Если фигура находится в группе или является фигурой комментария, она не будет удалена. |
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
| [Group](../../aspose.cells.drawing/shapecollection/group)(Shape[]) | Сгруппируйте фигуры. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int, int) |  |
| [Remove](../../aspose.cells.drawing/shapecollection/remove)(Shape) | Удалить фигуру. |
| [RemoveAt](../../aspose.cells.drawing/shapecollection/removeat#removeat)(int) | Удалить фигуру. (2 methods) |
| [Ungroup](../../aspose.cells.drawing/shapecollection/ungroup)(GroupShape) | Разгруппирует элементы формы. |
| [UpdateSelectedValue](../../aspose.cells.drawing/shapecollection/updateselectedvalue)() | Обновить выбранное значение значением связанной ячейки фигур. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();

  //получить ShapeCollection
ShapeCollection shapes = workbook.Worksheets[0].Shapes;

  //делай свое дело

  // Сохраняем файл Excel.
workbook.Save("result.xlsx");
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Shape](../shape)
* пространство имен [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
