---
title: Aspose.Cells.Charts
second_title: Справочник по Aspose.Cells для .NET API
description: Содержит все классы диаграмм и спарклайнов.
type: docs
weight: 20
url: /ru/net/aspose.cells.charts/
---
Содержит все классы диаграмм и спарклайнов.

## Классы

| Учебный класс | Описание |
| --- | --- |
| [Axis](./axis) | Инкапсулирует объект, представляющий ось диаграммы. |
| [AxisBins](./axisbins) | Представляет интервалы осей |
| [Chart](./chart) | Инкапсулирует объект, представляющий одну диаграмму Excel. |
| [ChartArea](./chartarea) | Инкапсулирует объект, представляющий область диаграммы на листе. |
| [ChartCollection](./chartcollection) | Инкапсулирует набор объектов[`Chart`](../aspose.cells.charts/chart). |
| [ChartDataTable](./chartdatatable) | Представляет таблицу данных диаграммы. |
| [ChartFrame](./chartframe) | Инкапсулирует объект, который представляет объект кадра на диаграмме. |
| [ChartGlobalizationSettings](./chartglobalizationsettings) | Представляет параметры глобализации для диаграммы. |
| [ChartPoint](./chartpoint) | Представляет одну точку в ряду на диаграмме. |
| [ChartPointCollection](./chartpointcollection) | Представляет коллекцию, содержащую все точки одной серии. |
| [ChartTextFrame](./charttextframe) | Инкапсулирует объект, представляющий объект кадра, содержащий текст. |
| [DataLabels](./datalabels) | Инкапсулирует коллекцию всех объектов DataLabel для указанной серии. |
| [DisplayUnitLabel](./displayunitlabel) | Представляет метку устройства отображения. |
| [DropBars](./dropbars) | Представляет столбцы вверх/вниз на диаграмме. |
| [ErrorBar](./errorbar) | Представляет планку ошибок ряда данных. |
| [Floor](./floor) | Инкапсулирует объект, представляющий нижнюю часть трехмерной диаграммы. |
| [Legend](./legend) | Инкапсулирует объект, представляющий легенду диаграммы. |
| [LegendEntry](./legendentry) | Представляет запись легенды в легенде диаграммы. |
| [LegendEntryCollection](./legendentrycollection) | Представляет коллекцию всех объектов[`LegendEntry`](../aspose.cells.charts/legendentry)в указанной легенде диаграммы. |
| [Marker](./marker) | Представляет маркер на линейной диаграмме, точечной диаграмме или лепестковой диаграмме. |
| [PivotOptions](./pivotoptions) | Представляет сложный тип, определяющий элементы управления разворотом, отображаемые на диаграмме |
| [PlotArea](./plotarea) | Инкапсулирует объект, представляющий область графика на диаграмме. |
| [Series](./series) | Инкапсулирует объект, представляющий один ряд данных на диаграмме. |
| [SeriesCollection](./seriescollection) | Инкапсулирует коллекцию объектов[`Series`](../aspose.cells.charts/series). |
| [SeriesLayoutProperties](./serieslayoutproperties) |  |
| [Sparkline](./sparkline) | Спарклайн представляет собой крошечную диаграмму или графику в ячейке рабочего листа, которая обеспечивает визуальное представление данных.  &lt;code&gt; [C#] Workbook book = new Workbook(); Рабочий лист = book.Worksheets[0]; лист.Ячейки["A1"].PutValue(5); лист.Ячейки["B1"].PutValue(2); лист.Ячейки["C1"].PutValue(1); лист.Ячейки["D1"].PutValue(3); // Определение CellArea CellArea ca = new CellArea(); ca.StartColumn = 4; ca.EndColumn = 4; ca.StartRow = 0; ca.EndRow = 0; int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, sheet.Name + "!A1:D1", false, ca); Группа SparklineGroup = лист.SparklineGroupCollection[idx]; idx = group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4); Спарклайн-линия = group.SparklineCollection[idx]; Console.WriteLine($"Диапазон данных Saprkline:{line.DataRange}, строка:{line.Row}, столбец:{line.Column}"); line.ToImage("output.png", new ImageOrPrintOptions()); &lt;/code&gt; |
| [SparklineCollection](./sparklinecollection) | Инкапсулирует набор объектов[`Sparkline`](../aspose.cells.charts/sparkline). |
| [SparklineGroup](./sparklinegroup) | [`Sparkline`](../aspose.cells.charts/sparkline)организован в группу спарклайнов. SparklineGroup содержит переменное количество элементов спарклайна. Группа спарклайнов определяет тип, настройки отображения и настройки осей для спарклайнов. |
| [SparklineGroupCollection](./sparklinegroupcollection) | Инкапсулирует коллекцию объектов[`SparklineGroup`](../aspose.cells.charts/sparklinegroup). |
| [TickLabelItem](./ticklabelitem) | Включить информацию об элементе Ticklabel |
| [TickLabels](./ticklabels) | Представляет метки делений, связанные с делениями на оси диаграммы. |
| [Title](./title) | Инкапсулирует объект, представляющий заголовок диаграммы или оси. |
| [Trendline](./trendline) | Представляет линию тренда на диаграмме. |
| [TrendlineCollection](./trendlinecollection) | Представляет набор всех объектов[`Trendline`](../aspose.cells.charts/trendline)для указанного ряда данных. |
| [Walls](./walls) | Инкапсулирует объект, представляющий стены трехмерной диаграммы. |
## перечисление

| перечисление | Описание |
| --- | --- |
| [AxisType](./axistype) | Представляет тип оси. |
| [BackgroundMode](./backgroundmode) | Представляет режим отображения фона. |
| [Bar3DShapeType](./bar3dshapetype) | Представляет форму, используемую с трехмерной гистограммой или гистограммой. |
| [BubbleSizeRepresents](./bubblesizerepresents) | Представляет, что представляет собой размер пузырька на пузырьковой диаграмме. |
| [CategoryType](./categorytype) | Представляет тип оси категорий. |
| [ChartLineFormattingType](./chartlineformattingtype) | Представляет тип формата линии графика. |
| [ChartMarkerType](./chartmarkertype) | Представляет стиль маркера на линейной диаграмме, точечной диаграмме или лепестковой диаграмме. |
| [ChartSplitType](./chartsplittype) | Представляет способ разделения двух частей круговой диаграммы или полосы круговой диаграммы. |
| [ChartTextDirectionType](./charttextdirectiontype) | Представляет тип направления текста диаграммы. |
| [ChartType](./charttype) | Перечисляет все типы диаграмм, используемые в Excel. |
| [CrossType](./crosstype) | Представляет перекрестный тип оси. |
| [DataLabelsSeparatorType](./datalabelsseparatortype) | Представляет тип разделителя DataLabels. |
| [DisplayUnitType](./displayunittype) | Представляет тип устройства отображения. |
| [ErrorBarDisplayType](./errorbardisplaytype) | Представляет тип отображения полосы ошибок. |
| [ErrorBarType](./errorbartype) | Представляет тип количества бара ошибок. |
| [FormattingType](./formattingtype) | Представляет тип форматирования, примененный к объекту[`Area`](../aspose.cells.drawing/area)или объекту[`Line`](../aspose.cells.drawing/line)объект. |
| [LabelPositionType](./labelpositiontype) | Представляет тип положения метки данных. |
| [LegendPositionType](./legendpositiontype) | Перечисляет типы позиций легенды. |
| [MapChartLabelLayout](./mapchartlabellayout) | Представляет макет меток карты. |
| [MapChartProjectionType](./mapchartprojectiontype) | Представляет тип проекции карты. |
| [MapChartRegionType](./mapchartregiontype) | Представляет тип региона карты. |
| [PlotDataByType](./plotdatabytype) | Представляет тип графика данных по строке или столбцу. |
| [PlotEmptyCellsType](./plotemptycellstype) | Представляет все пустые ячейки диаграммы. |
| [QuartileCalculationType](./quartilecalculationtype) | Представляет методы расчета квартилей. |
| [SparklineAxisMinMaxType](./sparklineaxisminmaxtype) | Представляет типы минимального и максимального значения для вертикальной оси спарклайна. |
| [SparklinePresetStyleType](./sparklinepresetstyletype) | Представляет предустановленные типы стиля для спарклайна. |
| [SparklineType](./sparklinetype) | Представляет типы спарклайнов. |
| [TickLabelPositionType](./ticklabelpositiontype) | Представляет тип положения меток деления на указанной оси. |
| [TickMarkType](./tickmarktype) | Представляет тип деления для указанной оси. |
| [TimeUnit](./timeunit) | Представляет базовую единицу для оси категорий. |
| [TrendlineType](./trendlinetype) | Представляет тип линии тренда. |

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
