---
title: LineFormat
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет все настройки линии.
type: docs
weight: 2220
url: /ru/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Представляет все настройки линии.

```csharp
public class LineFormat : FillFormat
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Получает и задает тип длины начальной стрелки линии. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Получает и задает тип стрелки начала линии. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Получает и задает тип начальной ширины стрелки линии. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Указывает конечные заглавные буквы. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Задает тип составной линии. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Определяет тип пунктира линии. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Получает и задает тип длины конечной стрелки линии. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Получает и задает тип конечной стрелки линии. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Получает и задает тип ширины конечной стрелки линии. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Получает и устанавливает тип заливки |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Возвращает цвет градиента 1 для указанной заливки. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Возвращает цвет градиента 2 для указанной заливки. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Возвращает тип цвета градиента для указанной заливки. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Возвращает степень градиента для указанной заливки. Применяется только для Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | получает[`GradientFill`](../fillformat/gradientfill) объект. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Возвращает стиль градиента для указанной заливки. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Возвращает вариант градиента для указанной заливки. Применяется только для Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Получает и устанавливает данные изображения изображения. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Указывает тип соединения линий. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Представляет шаблон отображения области. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | получает[`PatternFill`](../fillformat/patternfill) объект. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Получает и устанавливает тип формата изображения. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Возвращает заданный цвет градиента для указанной заливки. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Получает и задает масштаб формата изображения. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | получает[`SolidFill`](../fillformat/solidfill) объект. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Представляет тип текстуры для указанной заливки. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | получает[`TextureFill`](../fillformat/texturefill) объект. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Возвращает или задает степень прозрачности области в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Получает или задает вес линии в пунктах. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Определяет, имеет ли этот экземпляр то же значение, что и другой указанный[`LineFormat`](../lineformat) объект. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Получает хэш-код. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Задает для указанной заливки одноцветный градиент. Применяется только для Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Задает для указанной заливки заданный градиент цвета. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Устанавливает для указанной заливки двухцветный градиент. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Устанавливает для указанной заливки двухцветный градиент. Применяется только для Excel 2007. |

### Примеры

```csharp

[C#]
//Создание экземпляра объекта Workbook
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//делай свое дело

```

### Смотрите также

* class [FillFormat](../fillformat)
* пространство имен [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
