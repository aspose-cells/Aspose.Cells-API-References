---
title: "Класс SparklineGroup"
linktitle: "SparklineGroup"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SparklineGroup. Инкапсулирует объект, представляющий sparklinegroup в Go."
type: docs
weight: 200
url: /ru/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> организован в группу спарклайнов. SparklineGroup содержит переменное количество элементов спарклайна. Группа спарклайнов определяет тип, параметры отображения и настройки осей для спарклайнов.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | Сбрасывает диапазон данных и диапазон расположения группы спарклайнов. Этот метод очистит оригинальные элементы спарклайна в группе и создаст новые элементы спарклайна для новых диапазонов. |
| [GetPresetStyle](./getpresetstyle/) | Получает и задает тип предустановленного стиля группы спарклайнов. |
| [SetPresetStyle](./setpresetstyle/) | Получает и задает тип предустановленного стиля группы спарклайнов. |
| [GetSparklines](./getsparklines/) | Получает коллекцию объектов Sparkline. |
| [GetType](./gettype/) | Указывает тип спарклайна группы спарклайнов. |
| [SetType](./settype/) | Указывает тип спарклайна группы спарклайнов. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Указывает, как отображать пустые ячейки. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Указывает, как отображать пустые ячейки. |
| [GetDisplayHidden](./getdisplayhidden/) | Указывает, следует ли показывать данные в скрытых строках и столбцах. |
| [SetDisplayHidden](./setdisplayhidden/) | Указывает, следует ли показывать данные в скрытых строках и столбцах. |
| [GetShowHighPoint](./getshowhighpoint/) | Указывает, следует ли выделять самые высокие точки данных в группе спарклайнов. |
| [SetShowHighPoint](./setshowhighpoint/) | Указывает, следует ли выделять самые высокие точки данных в группе спарклайнов. |
| [GetHighPointColor](./gethighpointcolor/) | Получает и задает цвет самых высоких точек данных в группе спарклайнов. |
| [SetHighPointColor](./sethighpointcolor/) | Получает и задает цвет самых высоких точек данных в группе спарклайнов. |
| [GetShowLowPoint](./getshowlowpoint/) | Указывает, следует ли выделять самые низкие точки данных в группе спарклайнов. |
| [SetShowLowPoint](./setshowlowpoint/) | Указывает, следует ли выделять самые низкие точки данных в группе спарклайнов. |
| [GetLowPointColor](./getlowpointcolor/) | Получает и задает цвет самых низких точек данных в группе спарклайнов. |
| [SetLowPointColor](./setlowpointcolor/) | Получает и задает цвет самых низких точек данных в группе спарклайнов. |
| [GetShowNegativePoints](./getshownegativepoints/) | Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером. |
| [SetShowNegativePoints](./setshownegativepoints/) | Указывает, следует ли выделять отрицательные значения в группе спарклайнов другим цветом или маркером. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Получает и задает цвет отрицательных значений в группе спарклайнов. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Получает и задает цвет отрицательных значений в группе спарклайнов. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Указывает, следует ли выделять первую точку данных в группе спарклайнов. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Указывает, следует ли выделять первую точку данных в группе спарклайнов. |
| [GetFirstPointColor](./getfirstpointcolor/) | Получает и задает цвет первой точки данных в группе спарклайнов. |
| [SetFirstPointColor](./setfirstpointcolor/) | Получает и задает цвет первой точки данных в группе спарклайнов. |
| [GetShowLastPoint](./getshowlastpoint/) | Указывает, следует ли выделять последнюю точку данных в группе спарклайнов. |
| [SetShowLastPoint](./setshowlastpoint/) | Указывает, следует ли выделять последнюю точку данных в группе спарклайнов. |
| [GetLastPointColor](./getlastpointcolor/) | Получает и задает цвет последней точки данных в группе спарклайнов. |
| [SetLastPointColor](./setlastpointcolor/) | Получает и задает цвет последней точки данных в группе спарклайнов. |
| [GetShowMarkers](./getshowmarkers/) | Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов. |
| [SetShowMarkers](./setshowmarkers/) | Указывает, следует ли выделять каждую точку в каждом линейном спарклайне в группе спарклайнов. |
| [GetMarkersColor](./getmarkerscolor/) | Получает и задает цвет точек в каждом линейном спарклайне в группе спарклайнов. |
| [SetMarkersColor](./setmarkerscolor/) | Получает и задает цвет точек в каждом линейном спарклайне в группе спарклайнов. |
| [GetSeriesColor](./getseriescolor/) | Получает и задает цвет спарклайнов в группе спарклайнов. |
| [SetSeriesColor](./setseriescolor/) | Получает и задает цвет спарклайнов в группе спарклайнов. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Указывает, отображаются ли данные справа налево. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Указывает, отображаются ли данные справа налево. |
| [GetLineWeight](./getlineweight/) | Получает и задает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах пунктов. |
| [SetLineWeight](./setlineweight/) | Получает и задает толщину линии в каждом линейном спарклайне в группе спарклайнов, в единицах пунктов. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Получает и задает цвет горизонтальной оси в группе спарклайнов. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Получает и задает цвет горизонтальной оси в группе спарклайнов. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Указывает, следует ли отображать горизонтальную ось спарклайна. Горизонтальная ось появляется, если у спарклайна есть данные, пересекающие нулевую ось. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Указывает, следует ли отображать горизонтальную ось спарклайна. Горизонтальная ось появляется, если у спарклайна есть данные, пересекающие нулевую ось. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Представляет диапазон, содержащий значения дат для данных спарклайна. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Представляет диапазон, содержащий значения дат для данных спарклайна. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Представляет тип максимального значения вертикальной оси. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Представляет тип максимального значения вертикальной оси. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Получает и задает пользовательское максимальное значение для вертикальной оси. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Получает и задает пользовательское максимальное значение для вертикальной оси. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Задает пользовательское максимальное значение для вертикальной оси спарклайна с указанным типом значения оси. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Задает пользовательское минимальное значение для вертикальной оси спарклайна с указанным типом значения оси. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Представляет тип минимального значения вертикальной оси. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Представляет тип минимального значения вертикальной оси. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Получает и задает пользовательское минимальное значение для вертикальной оси. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Получает и задает пользовательское минимальное значение для вертикальной оси. |
