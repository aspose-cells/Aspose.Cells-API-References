---
title: "Класс LineFormat"
linktitle: "LineFormat"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс LineFormat. Инкапсулирует объект, представляющий lineformat в Go."
type: docs
weight: 200
url: /ru/go-cpp/lineformat/
---

## LineFormat class

Представляет все настройки линии.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLineFormat](./newlineformat/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetHashCode](./gethashcode/) | Получает хеш-код. |
| [Equals](./equals/) | Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект LineFormat. |
| [GetCompoundType](./getcompoundtype/) | Указывает тип соединения линии. |
| [SetCompoundType](./setcompoundtype/) | Указывает тип соединения линии. |
| [GetDashStyle](./getdashstyle/) | Указывает тип штриха линии. |
| [SetDashStyle](./setdashstyle/) | Указывает тип штриха линии. |
| [GetCapType](./getcaptype/) | Указывает конечные заглушки. |
| [SetCapType](./setcaptype/) | Указывает конечные заглушки. |
| [GetJoinType](./getjointype/) | Указывает тип соединения линии. |
| [SetJoinType](./setjointype/) | Указывает тип соединения линии. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Получает и задает тип начальной стрелки линии. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Получает и задает тип начальной стрелки линии. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Получает и задает тип ширины начальной стрелки линии. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Получает и задает тип ширины начальной стрелки линии. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | Получает и задает тип длины начальной стрелки линии. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | Получает и задает тип длины начальной стрелки линии. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | Получает и задает тип конечной стрелки линии. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | Получает и задает тип конечной стрелки линии. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | Получает и задает тип ширины конечной стрелки линии. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | Получает и задает тип ширины конечной стрелки линии. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | Получает и задает тип длины конечной стрелки линии. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | Получает и задает тип длины конечной стрелки линии. |
| [GetWeight](./getweight/) | Получает или задает толщину линии в пунктах. |
| [SetWeight](./setweight/) | Получает или задает толщину линии в пунктах. |
| [GetFillType](./getfilltype/) | Получает и задает тип заливки |
| [SetFillType](./setfilltype/) | Получает и задает тип заливки |
| [GetTransparency](./gettransparency/) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [SetTransparency](./settransparency/) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [GetGradientFill](./getgradientfill/) | Получает объект GradientFill. |
| [GetTextureFill](./gettexturefill/) | Получает объект TextureFill. |
| [GetSolidFill](./getsolidfill/) | Получает объект SolidFill. |
| [GetPatternFill](./getpatternfill/) | Получает объект PatternFill. |
| [GetGradientColorType](./getgradientcolortype/) | Возвращает тип градиентного цвета для указанной заливки. |
| [GetGradientStyle](./getgradientstyle/) | Возвращает стиль градиента для указанной заливки. |
| [GetGradientColor1](./getgradientcolor1/) | Возвращает градиентный цвет 1 для указанной заливки. |
| [GetGradientColor2](./getgradientcolor2/) | Возвращает градиентный цвет 2 для указанной заливки. |
| [GetGradientDegree](./getgradientdegree/) | Возвращает степень градиента для указанной заливки. Применяется только в Excel 2007. |
| [GetGradientVariant](./getgradientvariant/) | Возвращает вариант градиента для указанной заливки. Применяется только в Excel 2007. |
| [GetPresetColor](./getpresetcolor/) | Возвращает предустановленный градиентный цвет для указанной заливки. |
| [SetOneColorGradient](./setonecolorgradient/) | Устанавливает указанную заливку в одноцветный градиент. Применяется только к Excel 2007. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Устанавливает указанную заливку в двухцветный градиент. Применяется только к Excel 2007. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | Устанавливает указанную заливку в градиент предустановленного цвета. Применяется только для Excel 2007. |
| [GetTexture](./gettexture/) | Представляет тип текстуры для указанной заливки. |
| [SetTexture](./settexture/) | Представляет тип текстуры для указанной заливки. |
| [GetPattern](./getpattern/) | Представляет шаблон отображения области. |
| [SetPattern](./setpattern/) | Представляет шаблон отображения области. |
| [GetPictureFormatType](./getpictureformattype/) | Получает и задает тип формата изображения. |
| [SetPictureFormatType](./setpictureformattype/) | Получает и задает тип формата изображения. |
| [GetScale](./getscale/) | Получает и задает масштаб формата изображения. |
| [SetScale](./setscale/) | Получает и задает масштаб формата изображения. |
| [GetImageData](./getimagedata/) | Получает и задает данные изображения. |
| [SetImageData](./setimagedata/) | Получает и задает данные изображения. |
