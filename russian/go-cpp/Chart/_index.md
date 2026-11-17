---
title: "Класс Chart"
linktitle: "Chart"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Chart. Инкапсулирует объект, представляющий chart в Go."
type: docs
weight: 200
url: /ru/go-cpp/chart/
---

## Chart class

Инкапсулирует объект, представляющий отдельную диаграмму Excel.

```go

type Chart struct  {
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
| [GetStyle](./getstyle/) | Получает и задает встроенный стиль. |
| [SetStyle](./setstyle/) | Получает и задает встроенный стиль. |
| [GetChartObject](./getchartobject/) | Представляет chartShape; |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Указывает, скрывать ли кнопки полей сводчатой диаграммы только когда диаграмма является PivotChart. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Указывает, скрывать ли кнопки полей сводчатой диаграммы только когда диаграмма является PivotChart. |
| [GetPivotOptions](./getpivotoptions/) | Указывает элементы управления сводчатыми, которые отображаются на диаграмме. |
| [GetPivotSource](./getpivotsource/) | Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart. |
| [SetPivotSource](./setpivotsource/) | Источник — данные сводной таблицы. Если PivotSource не пуст, диаграмма является PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | Возвращает, относится ли ячейка к диаграмме. |
| [IsChartDataChanged](./ischartdatachanged/) | Определяет, изменился ли источник данных диаграммы. |
| [GetPlotBy](./getplotby/) | Получает и задает, строить ли график по строкам или столбцам. |
| [RefreshPivotData](./refreshpivotdata/) | Обновляет данные диаграммы из сводной таблицы. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Получает и задает, как отображать пустые ячейки. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Получает и задает, как отображать пустые ячейки. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Указывает, отображать ли только видимые ячейки. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Указывает, отображать ли только видимые ячейки. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | Указывает, отображать ли #N/A как пустое значение. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | Указывает, отображать ли #N/A как пустое значение. |
| [GetName](./getname/) | Получает и задает имя диаграммы. |
| [SetName](./setname/) | Получает и задает имя диаграммы. |
| [GetSizeWithWindow](./getsizewithwindow/) | Истина, если Microsoft Excel изменяет размер диаграммы, чтобы соответствовать размеру окна листа диаграммы. |
| [SetSizeWithWindow](./setsizewithwindow/) | Истина, если Microsoft Excel изменяет размер диаграммы, чтобы соответствовать размеру окна листа диаграммы. |
| [GetWorksheet](./getworksheet/) | Получает лист, содержащий эту диаграмму. |
| [GetShapes](./getshapes/) | Возвращает все графические фигуры в этой диаграмме. |
| [GetPrintSize](./getprintsize/) | Получает и задает размер печатной диаграммы. |
| [SetPrintSize](./setprintsize/) | Получает и задает размер печатной диаграммы. |
| [ChangeTemplate](./changetemplate/) | Измените тип диаграммы с помощью предустановленного шаблона. |
| [GetType](./gettype/) | Получает или задает тип диаграммы. |
| [SetType](./settype/) | Получает или задает тип диаграммы. |
| [Move](./move/) | Перемещает диаграмму в указанное место. |
| [GetNSeries](./getnseries/) | Получает коллекцию SeriesCollection, представляющую серии данных в диаграмме. |
| [GetFilteredNSeries](./getfilterednseries/) | Получает коллекцию SeriesCollection, представляющую отфильтрованные серии данных в диаграмме. |
| [GetTitle](./gettitle/) | Получает заголовок диаграммы. |
| [GetSubTitle](./getsubtitle/) | Получает подзаголовок диаграммы.Применяется только к файлам ODS. |
| [GetPlotArea](./getplotarea/) | Получает область построения диаграммы, включающую подписи делений осей. |
| [GetChartArea](./getchartarea/) | Получает область диаграммы в листе. |
| [GetCategoryAxis](./getcategoryaxis/) | Получает ось X диаграммы. |
| [GetValueAxis](./getvalueaxis/) | Получает ось Y диаграммы. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | Получает вторую ось Y диаграммы. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | Получает вторую ось X диаграммы. |
| [GetSeriesAxis](./getseriesaxis/) | Получает ось серии диаграммы. |
| [GetLegend](./getlegend/) | Получает легенду диаграммы. |
| [GetChartDataTable](./getchartdatatable/) | Представляет таблицу данных диаграммы. |
| [GetShowLegend](./getshowlegend/) | Получает или задает значение, указывающее, будет ли отображаться легенда диаграммы. По умолчанию true. |
| [SetShowLegend](./setshowlegend/) | Получает или задает значение, указывающее, будет ли отображаться легенда диаграммы. По умолчанию true. |
| [IsRectangularCornered](./isrectangularcornered/) | Получает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | Получает или задает значение, указывающее, имеет ли область диаграммы прямоугольные углы. По умолчанию true. |
| [GetShowDataTable](./getshowdatatable/) | Получает или задает значение, указывающее, отображает ли диаграмма таблицу данных. |
| [SetShowDataTable](./setshowdatatable/) | Получает или задает значение, указывающее, отображает ли диаграмма таблицу данных. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали).Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, от 0 до 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали).Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, от 0 до 360. |
| [GetGapWidth](./getgapwidth/) | Возвращает или задает расстояние между группами столбцов или колонок в процентах от их ширины.Значение этого свойства должно быть от 0 до 500. |
| [SetGapWidth](./setgapwidth/) | Возвращает или задает расстояние между группами столбцов или колонок в процентах от их ширины.Значение этого свойства должно быть от 0 до 500. |
| [GetGapDepth](./getgapdepth/) | Получает или задает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера.Значение этого свойства должно быть от 0 до 500. |
| [SetGapDepth](./setgapdepth/) | Получает или задает расстояние между сериями данных в 3‑D диаграмме в процентах от ширины маркера.Значение этого свойства должно быть от 0 до 500. |
| [Calculate](./calculate/) | Вычисляет пользовательские позиции области построения и осей, если их позиции назначаются автоматически. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Вычисляет пользовательскую позицию области построения и осей, если их позиция назначена автоматически, с параметрами расчёта диаграммы. |
| [GetFloor](./getfloor/) | Возвращает объект Floor, представляющий стены 3‑D диаграммы. |
| [GetWalls](./getwalls/) | Возвращает объект Walls, представляющий стены 3‑D диаграммы. |
| [GetBackWall](./getbackwall/) | Возвращает объект Walls, представляющий заднюю стену 3‑D диаграммы. |
| [GetSideWall](./getsidewall/) | Возвращает объект Walls, представляющий боковую стену 3‑D диаграммы. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | Истина, если сетка рисуется в двумерном виде на 3‑D диаграмме. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | Истина, если сетка рисуется в двумерном виде на 3‑D диаграмме. |
| [GetRotationAngle](./getrotationangle/) | Представляет вращение вида 3‑D диаграммы (вращение области построения вокруг оси Z в градусах). |
| [SetRotationAngle](./setrotationangle/) | Представляет вращение вида 3‑D диаграммы (вращение области построения вокруг оси Z в градусах). |
| [GetElevation](./getelevation/) | Представляет высоту (угол наклона) вида 3‑D диаграммы в градусах. |
| [SetElevation](./setelevation/) | Представляет высоту (угол наклона) вида 3‑D диаграммы в градусах. |
| [GetRightAngleAxes](./getrightangleaxes/) | Истина, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм). |
| [SetRightAngleAxes](./setrightangleaxes/) | Истина, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм). |
| [GetAutoScaling](./getautoscaling/) | Истина, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. Свойство RightAngleAxes должно быть истинным. |
| [SetAutoScaling](./setautoscaling/) | Истина, если Microsoft Excel масштабирует 3‑D диаграмму так, чтобы её размер был ближе к эквивалентной 2‑D диаграмме. Свойство RightAngleAxes должно быть истинным. |
| [GetHeightPercent](./getheightpercent/) | Возвращает или задаёт высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 %). |
| [SetHeightPercent](./setheightpercent/) | Возвращает или задаёт высоту 3‑D диаграммы в процентах от её ширины (от 5 до 500 %). |
| [GetPerspective](./getperspective/) | Возвращает или задаёт перспективу трехмерного вида диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes истинно. |
| [SetPerspective](./setperspective/) | Возвращает или задаёт перспективу трехмерного вида диаграммы. Должно быть от 0 до 100. Это свойство игнорируется, если свойство RightAngleAxes истинно. |
| [GetIs3D](./getis3d/) | Указывает, является ли диаграмма 3‑D. |
| [GetDepthPercent](./getdepthpercent/) | Представляет глубину 3‑D диаграммы в процентах от её ширины (от 20 до 2000 %). |
| [SetDepthPercent](./setdepthpercent/) | Представляет глубину 3‑D диаграммы в процентах от её ширины (от 20 до 2000 %). |
| [ToImage_String](./toimage_string/) | Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | Создаёт изображение диаграммы и сохраняет его в файл указанного типа изображения. |
| [ToImage_Int64](./toimage_int64/) | Создаёт изображение диаграммы и сохраняет его в поток в формате JPEG. |
| [ToImage_ImageType](./toimage_imagetype/) | Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [ToPdf_String](./topdf_string/) | Сохраняет диаграмму в PDF‑файл. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Сохраняет диаграмму в PDF‑файл. |
| [ToPdf](./topdf/) | Создаёт PDF‑файл диаграммы и сохраняет его в поток. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Создаёт PDF‑файл диаграммы и сохраняет его в поток. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Создаёт изображение диаграммы и сохраняет его в поток в указанном формате. |
| [GetActualSize](./getactualsize/) | Получает фактический размер диаграммы в пикселях. |
| [GetPlacement](./getplacement/) | Представляет способ привязки диаграммы к ячейкам под ней. |
| [SetPlacement](./setplacement/) | Представляет способ привязки диаграммы к ячейкам под ней. |
| [GetPageSetup](./getpagesetup/) | Представляет описание параметров страницы в этой диаграмме. |
| [HasAxis](./hasaxis/) | Возвращает, какие оси присутствуют на диаграмме. |
| [SwitchRowColumn](./switchrowcolumn/) | Переключает строки/столбцы. |
| [GetChartDataRange](./getchartdatarange/) | Получает диапазон источника данных диаграммы. |
| [SetChartDataRange](./setchartdatarange/) | Указывает диапазон данных для диаграммы. |
| [GetLine](./getline/) | Получает линию. |
