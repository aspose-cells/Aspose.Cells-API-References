---
title: "ChartArea класс"
linktitle: "ChartArea"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "ChartArea класс. Инкапсулирует объект, представляющий chartarea в Go."
type: docs
weight: 200
url: /ru/go-cpp/chartarea/
---

## ChartArea class

Инкапсулирует объект, представляющий область диаграммы в листе.

```go

type ChartArea struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewChartArea](./newchartarea/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | Получает или задает горизонтальное смещение от столбца верхнего левого угла, как отношение к области диаграммы. |
| [SetXRatioToChart](./setxratiotochart/) | Получает или задает горизонтальное смещение от столбца верхнего левого угла, как отношение к области диаграммы. |
| [GetYRatioToChart](./getyratiotochart/) | Получает или получает вертикальное смещение от строки верхнего левого угла, в единицах отношения к области диаграммы. |
| [SetYRatioToChart](./setyratiotochart/) | Получает или получает вертикальное смещение от строки верхнего левого угла, в единицах отношения к области диаграммы. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Получает или задает вертикальное смещение от строки нижнего правого угла, в единицах отношения к области диаграммы. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Получает или задает вертикальное смещение от строки нижнего правого угла, в единицах отношения к области диаграммы. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Получает или задает горизонтальное смещение от столбца нижнего правого угла, в единицах отношения к области диаграммы. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Получает или задает горизонтальное смещение от столбца нижнего правого угла, в единицах отношения к области диаграммы. |
| [GetFont](./getfont/) | Получает объект Font указанного объекта ChartArea. |
| [IsInnerMode](./isinnermode/) | Указывает, включает ли размер области построения отметки делений и подписи осей. False указывает, что размер определяет размер области построения, отметок делений и подписей осей. |
| [SetIsInnerMode](./setisinnermode/) | Указывает, включает ли размер области построения отметки делений и подписи осей. False указывает, что размер определяет размер области построения, отметок делений и подписей осей. |
| [GetShadow](./getshadow/) | True, если у кадра есть тень. |
| [SetShadow](./setshadow/) | True, если у кадра есть тень. |
| [GetShapeProperties](./getshapeproperties/) | Получает объект ShapeProperties. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Представляет x позиции по умолчанию в единицах доли области диаграммы. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Представляет y позиции по умолчанию в единицах доли области диаграммы. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Представляет ширину позиции по умолчанию в единицах доли области диаграммы. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Представляет высоту позиции по умолчанию в единицах доли области диаграммы. |
| [GetBorder](./getborder/) | Получает Line</see>. |
| [GetArea](./getarea/) | Получает Area</see>. |
| [GetTextOptions](./gettextoptions/) | Получает и задает параметры текста. |
| [GetAutoScaleFont](./getautoscalefont/) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [SetAutoScaleFont](./setautoscalefont/) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [IsAutomaticSize](./isautomaticsize/) | Указывает, автоматически ли размеряется рамка диаграммы. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Указывает, автоматически ли размеряется рамка диаграммы. |
| [GetXPixel](./getxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [SetXPixel](./setxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [GetYPixel](./getypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [SetYPixel](./setypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [GetWidthPixel](./getwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [SetWidthPixel](./setwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [GetHeightPixel](./getheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
| [SetHeightPixel](./setheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
| [SetPositionAuto](./setpositionauto/) | Установить позицию кадра в автоматический режим |
