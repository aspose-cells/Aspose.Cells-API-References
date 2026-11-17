---
title: "DataLabels Класс"
linktitle: "DataLabels"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "DataLabels класс. Инкапсулирует объект, представляющий datalabels в Go."
type: docs
weight: 200
url: /ru/go-cpp/datalabels/
---

## DataLabels class

Инкапсулирует коллекцию всех объектов DataLabel для указанной серии.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetBorder](./getborder/) | Получает Line</see>. |
| [GetArea](./getarea/) | Получает Area</see>. |
| [IsAutoText](./isautotext/) | Указывает, что текст сгенерирован автоматически. |
| [SetIsAutoText](./setisautotext/) | Указывает, что текст сгенерирован автоматически. |
| [GetDirectionType](./getdirectiontype/) | Получает и задает направление текста. |
| [SetDirectionType](./setdirectiontype/) | Получает и задает направление текста. |
| [GetText](./gettext/) | Получает или задает текст метки данных. |
| [SetText](./settext/) | Получает или задает текст метки данных. |
| [IsTextWrapped](./istextwrapped/) | Получает или задает значение, указывающее, перенесён ли текст. |
| [SetIsTextWrapped](./setistextwrapped/) | Получает или задает значение, указывающее, перенесён ли текст. |
| [GetBackgroundMode](./getbackgroundmode/) | Получает и задает режим отображения фона |
| [SetBackgroundMode](./setbackgroundmode/) | Получает и задает режим отображения фона |
| [GetShowValue](./getshowvalue/) | Представляет поведение отображения значений меток данных указанной диаграммы. True отображает значения. False скрывает их. |
| [SetShowValue](./setshowvalue/) | Представляет поведение отображения значений меток данных указанной диаграммы. True отображает значения. False скрывает их. |
| [GetShowCellRange](./getshowcellrange/) | Указывает, следует ли показывать диапазон ячеек в качестве меток данных. |
| [SetShowCellRange](./setshowcellrange/) | Указывает, следует ли показывать диапазон ячеек в качестве меток данных. |
| [GetShowPercentage](./getshowpercentage/) | Представляет поведение отображения процентного значения меток данных указанной диаграммы. True отображает процентное значение. False скрывает его. |
| [SetShowPercentage](./setshowpercentage/) | Представляет поведение отображения процентного значения меток данных указанной диаграммы. True отображает процентное значение. False скрывает его. |
| [GetShowBubbleSize](./getshowbubblesize/) | Представляет поведение отображения процентного значения меток данных указанной диаграммы. True отображает процентное значение. False скрывает процентное значение. |
| [SetShowBubbleSize](./setshowbubblesize/) | Представляет поведение отображения процентного значения меток данных указанной диаграммы. True отображает процентное значение. False скрывает процентное значение. |
| [GetShowCategoryName](./getshowcategoryname/) | Представляет поведение отображения названия категории меток данных указанной диаграммы. True отображает название категории для меток данных на диаграмме. False скрывает его. |
| [SetShowCategoryName](./setshowcategoryname/) | Представляет поведение отображения названия категории меток данных указанной диаграммы. True отображает название категории для меток данных на диаграмме. False скрывает его. |
| [GetShowSeriesName](./getshowseriesname/) | Указывает, отображается ли имя серии в метках данных на диаграмме. True показывает имя серии. False скрывает его. |
| [SetShowSeriesName](./setshowseriesname/) | Указывает, отображается ли имя серии в метках данных на диаграмме. True показывает имя серии. False скрывает его. |
| [GetShowLegendKey](./getshowlegendkey/) | Представляет поведение отображения ключа легенды меток данных указанной диаграммы. True, если ключ легенды меток данных виден. |
| [SetShowLegendKey](./setshowlegendkey/) | Представляет поведение отображения ключа легенды меток данных указанной диаграммы. True, если ключ легенды меток данных виден. |
| [Get_NumberFormat](./get_numberformat/) | Представляет строку формата для объекта DataLabels. |
| [SetNumberFormat](./setnumberformat/) | Представляет строку формата для объекта DataLabels. |
| [GetNumber](./getnumber/) | Получает и задает встроенный числовой формат. |
| [SetNumber](./setnumber/) | Получает и задает встроенный числовой формат. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | Истина, если числовой формат связан с ячейками (так, что формат числа меняется в метках, когда меняется в ячейках). |
| [SetNumberFormatLinked](./setnumberformatlinked/) | Истина, если числовой формат связан с ячейками (так, что формат числа меняется в метках, когда меняется в ячейках). |
| [ApplyFont](./applyfont/) | Применить шрифт меток данных ко всем дочерним узлам. |
| [GetFont](./getfont/) | Получает шрифт DataLabels; |
| [GetSeparatorType](./getseparatortype/) | Получает или задает тип разделителя, используемый для меток данных на диаграмме. |
| [SetSeparatorType](./setseparatortype/) | Получает или задает тип разделителя, используемый для меток данных на диаграмме. |
| [GetSeparatorValue](./getseparatorvalue/) | Получает или задает значение разделителя, используемого для подписей данных на диаграмме. |
| [SetSeparatorValue](./setseparatorvalue/) | Получает или задает значение разделителя, используемого для подписей данных на диаграмме. |
| [GetPosition](./getposition/) | Представляет положение подписи данных. |
| [SetPosition](./setposition/) | Представляет положение подписи данных. |
| [IsNeverOverlap](./isneveroverlap/) | Указывает, не перекрываются ли подписи данных при преобразовании круговой диаграммы в изображение. Примечание: это свойство имеет смысл только при преобразовании круговой диаграммы в изображение. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Указывает, не перекрываются ли подписи данных при преобразовании круговой диаграммы в изображение. Примечание: это свойство имеет смысл только при преобразовании круговой диаграммы в изображение. |
| [GetShapeType](./getshapetype/) | Получает или задает тип формы подписи данных. |
| [SetShapeType](./setshapetype/) | Получает или задает тип формы подписи данных. |
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
| [GetTextOptions](./gettextoptions/) | Получает и задает параметры текста. |
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
| [GetLinkedSource](./getlinkedsource/) | Получает и задает ссылку на лист. |
| [SetLinkedSource](./setlinkedsource/) | Получает и задает ссылку на лист. |
