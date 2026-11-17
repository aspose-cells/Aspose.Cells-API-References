---
title: "Класс Axis"
linktitle: "Axis"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Axis. Инкапсулирует объект, представляющий ось в Go."
type: docs
weight: 200
url: /ru/go-cpp/axis/
---

## Axis class

Инкапсулирует объект, представляющий ось диаграммы.

```go

type Axis struct  {
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
| [GetArea](./getarea/) | Получает область. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Указывает, назначается ли минимальное значение автоматически. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Указывает, назначается ли минимальное значение автоматически. |
| [GetMinValue](./getminvalue/) | Представляет минимальное значение на оси значений. |
| [SetMinValue](./setminvalue/) | Представляет минимальное значение на оси значений. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Указывает, назначается ли максимальное значение автоматически. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Указывает, назначается ли максимальное значение автоматически. |
| [GetMaxValue](./getmaxvalue/) | Представляет максимальное значение на оси значений. |
| [SetMaxValue](./setmaxvalue/) | Представляет максимальное значение на оси значений. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Указывает, назначается ли основной делитель оси автоматически. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Указывает, назначается ли основной делитель оси автоматически. |
| [GetMajorUnit](./getmajorunit/) | Представляет основные единицы измерения оси. |
| [SetMajorUnit](./setmajorunit/) | Представляет основные единицы измерения оси. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Указывает, назначается ли вспомогательный делитель оси автоматически. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Указывает, назначается ли вспомогательный делитель оси автоматически. |
| [GetMinorUnit](./getminorunit/) | Представляет вспомогательные единицы измерения оси. |
| [SetMinorUnit](./setminorunit/) | Представляет вспомогательные единицы измерения оси. |
| [GetAxisLine](./getaxisline/) | Получает внешний вид оси. |
| [GetMajorTickMark](./getmajortickmark/) | Представляет тип основной метки деления для указанной оси. |
| [SetMajorTickMark](./setmajortickmark/) | Представляет тип основной метки деления для указанной оси. |
| [GetMinorTickMark](./getminortickmark/) | Представляет тип вспомогательной метки деления для указанной оси. |
| [SetMinorTickMark](./setminortickmark/) | Представляет тип вспомогательной метки деления для указанной оси. |
| [GetTickLabelPosition](./getticklabelposition/) | Представляет положение подписей меток деления на указанной оси. |
| [SetTickLabelPosition](./setticklabelposition/) | Представляет положение подписей меток деления на указанной оси. |
| [GetCrossAt](./getcrossat/) | Представляет точку на оси значений, где ось категорий её пересекает. |
| [SetCrossAt](./setcrossat/) | Представляет точку на оси значений, где ось категорий её пересекает. |
| [GetCrossType](./getcrosstype/) | Представляет тип пересечения (CrossType) на указанной оси, где другая ось её пересекает. |
| [SetCrossType](./setcrosstype/) | Представляет тип пересечения (CrossType) на указанной оси, где другая ось её пересекает. |
| [GetLogBase](./getlogbase/) | Представляет логарифмическую основу. Значение по умолчанию — 10. |
| [SetLogBase](./setlogbase/) | Представляет логарифмическую основу. Значение по умолчанию — 10. |
| [IsLogarithmic](./islogarithmic/) | Указывает, является ли тип шкалы оси значений логарифмическим. |
| [SetIsLogarithmic](./setislogarithmic/) | Указывает, является ли тип шкалы оси значений логарифмическим. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Указывает, отображает ли Microsoft Excel точки данных от последней к первой. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Указывает, отображает ли Microsoft Excel точки данных от последней к первой. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Представляет, пересекает ли ось значений ось категорий между категориями. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Представляет, пересекает ли ось значений ось категорий между категориями. |
| [GetTickLabels](./getticklabels/) | Возвращает объект TickLabels, представляющий подписи делений для указанной оси. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Представляет количество категорий или рядов между подписями делений. Применяется только к осям категорий и рядов. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Представляет количество категорий или рядов между подписями делений. Применяется только к осям категорий и рядов. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Указывает, является ли интервал подписи деления автоматическим |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Указывает, является ли интервал подписи деления автоматическим |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Возвращает или задает количество категорий или рядов между делениями. Применяется только к осям категорий и рядов. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Возвращает или задает количество категорий или рядов между делениями. Применяется только к осям категорий и рядов. |
| [GetDisplayUnit](./getdisplayunit/) | Представляет подпись единицы измерения для указанной оси. |
| [SetDisplayUnit](./setdisplayunit/) | Представляет подпись единицы измерения для указанной оси. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Указывает пользовательское значение для отображаемой единицы. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Указывает пользовательское значение для отображаемой единицы. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Представляет подпись единицы измерения на оси в указанной диаграмме. Подписи единиц полезны при построении больших значений — например, в миллионах или миллиардах. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Представляет, отображается ли подпись единицы измерения на указанной оси. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Представляет, отображается ли подпись единицы измерения на указанной оси. |
| [GetTitle](./gettitle/) | Получает заголовок этой оси в диаграмме. |
| [GetCategoryType](./getcategorytype/) | Представляет тип оси категорий. |
| [SetCategoryType](./setcategorytype/) | Представляет тип оси категорий. |
| [GetBaseUnitScale](./getbaseunitscale/) | Представляет масштаб базовой единицы для оси категорий. |
| [SetBaseUnitScale](./setbaseunitscale/) | Представляет масштаб базовой единицы для оси категорий. |
| [GetMajorUnitScale](./getmajorunitscale/) | Представляет масштаб основной единицы для оси категорий. |
| [SetMajorUnitScale](./setmajorunitscale/) | Представляет масштаб основной единицы для оси категорий. |
| [GetMinorUnitScale](./getminorunitscale/) | Представляет масштаб основной единицы для оси категорий. |
| [SetMinorUnitScale](./setminorunitscale/) | Представляет масштаб основной единицы для оси категорий. |
| [IsVisible](./isvisible/) | Представляет, видна ли ось. |
| [SetIsVisible](./setisvisible/) | Представляет, видна ли ось. |
| [GetMajorGridLines](./getmajorgridlines/) | Представляет основные линии сетки на оси диаграммы. |
| [GetMinorGridLines](./getminorgridlines/) | Представляет вспомогательные линии сетки на оси диаграммы. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Указывает, должны ли подписи отображаться многоуровнево. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Указывает, должны ли подписи отображаться многоуровнево. |
| [GetAxisTexts](./getaxistexts/) | Получает подписи оси после вызова метода Chart.Calculate(). |
| [GetBins](./getbins/) | Представляет интервалы (bins) на оси диаграммы (гистограмма/Пирто) |
