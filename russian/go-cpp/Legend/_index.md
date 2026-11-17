---
title: "Класс Legend"
linktitle: "Легенда"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Legend. Инкапсулирует объект, представляющий легенду в Go."
type: docs
weight: 200
url: /ru/go-cpp/legend/
---

## Legend class

Инкапсулирует объект, представляющий легенду диаграммы.

```go

type Legend struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLegend](./newlegend/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetPosition](./getposition/) | Получает или задает тип положения легенды. |
| [SetPosition](./setposition/) | Получает или задает тип положения легенды. |
| [GetLegendEntries](./getlegendentries/) | Получает коллекцию всех объектов LegendEntry в указанной легенде диаграммы.Установка записей легенды для поверхностной диаграммы не поддерживается.Так будет возвращён null, если тип диаграммы — тип поверхностной диаграммы. |
| [GetLegendLabels](./getlegendlabels/) | Получает подписи записей легенды после вызова метода Chart.Calculate(). |
| [IsOverLay](./isoverlay/) | Получает или задает, показывать ли легенду без наложения на диаграмму. |
| [SetIsOverLay](./setisoverlay/) | Получает или задает, показывать ли легенду без наложения на диаграмму. |
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
| [IsAutomaticSize](./isautomaticsize/) | Указывает, автоматически ли размеряется рамка диаграммы. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Указывает, автоматически ли размеряется рамка диаграммы. |
| [GetXRatioToChart](./getxratiotochart/) | Получает или задает координату x верхнего левого угла в единицах отношения к области диаграммы. |
| [SetXRatioToChart](./setxratiotochart/) | Получает или задает координату x верхнего левого угла в единицах отношения к области диаграммы. |
| [GetYRatioToChart](./getyratiotochart/) | Получает или задает координату y верхнего левого угла в единицах отношения области диаграммы. |
| [SetYRatioToChart](./setyratiotochart/) | Получает или задает координату y верхнего левого угла в единицах отношения области диаграммы. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Получает или задает ширину кадра в единицах отношения области диаграммы. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Получает или задает ширину кадра в единицах отношения области диаграммы. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Получает или задает высоту кадра в единицах отношения области диаграммы. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Получает или задает высоту кадра в единицах отношения области диаграммы. |
| [GetXPixel](./getxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [SetXPixel](./setxpixel/) | Получает или задает координату x верхнего левого угла в единицах пикселей. |
| [GetYPixel](./getypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [SetYPixel](./setypixel/) | Получает или задает координату y верхнего левого угла в единицах пикселей. |
| [GetWidthPixel](./getwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [SetWidthPixel](./setwidthpixel/) | Получает или задает ширину кадра в единицах пикселей. |
| [GetHeightPixel](./getheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
| [SetHeightPixel](./setheightpixel/) | Получает или задает высоту кадра в единицах пикселей. |
| [SetPositionAuto](./setpositionauto/) | Установить позицию кадра в автоматический режим |
| [IsDeleted](./isdeleted/) | Указывает, удалена ли эта метка данных. |
| [SetIsDeleted](./setisdeleted/) | Указывает, удалена ли эта метка данных. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Получает и задает горизонтальное выравнивание текста. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Получает и задает горизонтальное выравнивание текста. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Получает или задает вертикальное выравнивание текста. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Получает или задает вертикальное выравнивание текста. |
| [GetRotationAngle](./getrotationangle/) | Представляет угол поворота текста. |
| [SetRotationAngle](./setrotationangle/) | Представляет угол поворота текста. |
| [IsAutomaticRotation](./isautomaticrotation/) | Указывает, автоматически ли поворачивается текст диаграммы. |
| [Characters](./characters/) | Возвращает объект Characters, представляющий диапазон символов в тексте. |
| [GetReadingOrder](./getreadingorder/) | Представляет порядок чтения текста. |
| [SetReadingOrder](./setreadingorder/) | Представляет порядок чтения текста. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Получает или задает, должна ли фигура автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это когда текст внутри фигуры масштабируется, чтобы вместить весь текст. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Получает или задает, должна ли фигура автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это когда текст внутри фигуры масштабируется, чтобы вместить весь текст. |
| [IsAutoText](./isautotext/) | Указывает, что текст сгенерирован автоматически. |
| [SetIsAutoText](./setisautotext/) | Указывает, что текст сгенерирован автоматически. |
| [GetText](./gettext/) | Получает или задает текст заголовка кадра. |
| [SetText](./settext/) | Получает или задает текст заголовка кадра. |
| [GetLinkedSource](./getlinkedsource/) | Получает и задает ссылку на лист. |
| [SetLinkedSource](./setlinkedsource/) | Получает и задает ссылку на лист. |
| [GetDirectionType](./getdirectiontype/) | Получает и задает направление текста. |
| [SetDirectionType](./setdirectiontype/) | Получает и задает направление текста. |
| [IsTextWrapped](./istextwrapped/) | Получает или задает значение, указывающее, перенесён ли текст. |
| [SetIsTextWrapped](./setistextwrapped/) | Получает или задает значение, указывающее, перенесён ли текст. |
