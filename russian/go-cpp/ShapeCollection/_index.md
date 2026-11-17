---
title: "Класс ShapeCollection"
linktitle: "ShapeCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ShapeCollection. Инкапсулирует объект, представляющий shapecollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/shapecollection/
---

## ShapeCollection class

Представляет все фигуры в листе/диаграмме.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Get_Int](./get_int/) | Получает объект Shape по указанному индексу в списке. |
| [Get_String](./get_string/) | Получает объект Shape по имени фигуры. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Добавляет и копирует shape в лист. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Добавляет и копирует shape в лист. |
| [AddCheckBox](./addcheckbox/) | Добавляет флажок в лист. |
| [AddTextBox](./addtextbox/) | Добавляет текстовое поле в лист. |
| [AddEquation](./addequation/) | Добавляет объект уравнения в лист. |
| [AddLaTeXEquation](./addlatexequation/) | Добавляет объект уравнения в лист с использованием строк формата LaTeX. |
| [AddSpinner](./addspinner/) | Добавляет элемент Spinner в лист. |
| [AddScrollBar](./addscrollbar/) | Добавляет элемент ScrollBar в лист. |
| [AddRadioButton](./addradiobutton/) | Добавляет элемент RadioButton в лист. |
| [AddListBox](./addlistbox/) | Добавляет элемент ListBox в лист. |
| [AddComboBox](./addcombobox/) | Добавляет элемент ComboBox в лист. |
| [AddGroupBox](./addgroupbox/) | Добавляет элемент GroupBox в лист. |
| [AddButton](./addbutton/) | Добавляет элемент Button в лист. |
| [AddLabel](./addlabel/) | Добавляет элемент Label в лист. |
| [AddLabelInChart](./addlabelinchart/) | Добавляет метку в диаграмму. |
| [AddTextBoxInChart](./addtextboxinchart/) | Добавляет текстовое поле в диаграмму. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Вставляет объект WordArt в диаграмму. |
| [AddTextEffect](./addtexteffect/) | Вставляет объект WordArt. |
| [AddWordArt](./addwordart/) | Добавляет предустановленный WordArt, начиная с Excel 2007. |
| [AddRectangle](./addrectangle/) | Добавляет объект RectangleShape в лист. |
| [AddOval](./addoval/) | Добавляет объект Oval в лист. |
| [AddLine](./addline/) | Добавляет объект LineShape в лист. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Добавляет свободно плавающую форму в лист. Применяется только к линиям/изображениям. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Добавляет форму в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Добавляет форму в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Добавляет форму в диаграмму. Все единицы — процентный масштаб области диаграммы. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Добавляет форму в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [AddArc](./addarc/) | Добавляет объект ArcShape в лист. |
| [AddShape](./addshape/) | Добавляет объект Shape в лист. |
| [AddAutoShape](./addautoshape/) | Добавляет объект AutoShape в лист. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Добавляет объект AutoShape в диаграмму. |
| [AddActiveXControl](./addactivexcontrol/) | Создает элемент управления Activex. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Добавляет изображение в коллекцию. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Добавляет изображение в коллекцию. |
| [AddSvg](./addsvg/) | Добавляет SVG‑изображение. |
| [AddIcons](./addicons/) | Добавляет SVG‑изображение. |
| [AddLinkedPicture](./addlinkedpicture/) | Добавить связанную картинку. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Добавить связанную картинку. |
| [AddPictureInChart](./addpictureinchart/) | Добавляет изображение в диаграмму. |
| [AddOleObject](./addoleobject/) | Добавляет объект OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | Копировать все комментарии в диапазоне. |
| [CopyInRange](./copyinrange/) | Копировать фигуры в диапазоне в целевой диапазон. |
| [DeleteInRange](./deleteinrange/) | Удалить фигуры в диапазоне. Фигуры‑комментарии не будут удалены. |
| [DeleteShape](./deleteshape/) | Удалить фигуру. Если фигура находится в группе или является фигурой‑комментарием, она не будет удалена. |
| [Group](./group/) | Сгруппировать фигуры. |
| [Ungroup](./ungroup/) | Разгруппировать элементы фигур. |
| [RemoveAt](./removeat/) | Удалить фигуру. |
| [Remove](./remove/) | Удалить фигуру. |
| [Clear](./clear/) | Очистить все фигуры на листе. |
| [UpdateSelectedValue](./updateselectedvalue/) | Обновить выбранное значение значением связанной ячейки или диапазона фигуры. |
| [AddFreeform](./addfreeform/) | Добавляет произвольную форму на лист. |
| [AddSignatureLine](./addsignatureline/) | Добавляет строку подписи на лист. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
