---
title: "Класс PlotArea"
linktitle: "PlotArea"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PlotArea. Инкапсулирует объект, представляющий область построения (plotarea) в Go."
type: docs
weight: 200
url: /ru/go-cpp/plotarea/
---

## PlotArea class

Инкапсулирует объект, представляющий область построения диаграммы.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPlotArea](./newplotarea/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | Получает или задаёт координату x верхнего левого угла ограничивающего прямоугольника области построения в виде отношения к области диаграммы. |
| [SetXRatioToChart](./setxratiotochart/) | Получает или задаёт координату x верхнего левого угла ограничивающего прямоугольника области построения в виде отношения к области диаграммы. |
| [GetYRatioToChart](./getyratiotochart/) | Получает или задаёт координату y верхнего верхнего угла ограничивающего прямоугольника области построения в виде отношения к области диаграммы. |
| [SetYRatioToChart](./setyratiotochart/) | Получает или задаёт координату y верхнего верхнего угла ограничивающего прямоугольника области построения в виде отношения к области диаграммы. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Получает или задаёт высоту ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Получает или задаёт высоту ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Получает или задаёт ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Получает или задаёт ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | Получает или получает координату x верхнего верхнего угла области построения в единицах отношения к области диаграммы. |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | Получает или получает координату x верхнего верхнего угла области построения в единицах отношения к области диаграммы. |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | Получает или получает координату x верхнего верхнего угла области построения в единицах отношения к области диаграммы. |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | Получает или получает координату x верхнего верхнего угла области построения в единицах отношения к области диаграммы. |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | Получает или задаёт высоту области построения в единицах отношения к области диаграммы. |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | Получает или задаёт высоту области построения в единицах отношения к области диаграммы. |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | Получает или задает ширину области построения в единицах отношения к области диаграммы. |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | Получает или задает ширину области построения в единицах отношения к области диаграммы. |
| [SetPositionAuto](./setpositionauto/) | Установить позицию области построения в автоматический режим |
| [IsAutomaticSize](./isautomaticsize/) | Указывает, автоматически ли задаются размеры области построения. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Указывает, автоматически ли задаются размеры области построения. |
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
| [GetFont](./getfont/) | Получает объект Font указанного объекта ChartFrame. |
| [GetAutoScaleFont](./getautoscalefont/) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [SetAutoScaleFont](./setautoscalefont/) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. |
| [GetXPixel](./getxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [SetXPixel](./setxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [GetYPixel](./getypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [SetYPixel](./setypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [GetWidthPixel](./getwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [SetWidthPixel](./setwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [GetHeightPixel](./getheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
| [SetHeightPixel](./setheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
