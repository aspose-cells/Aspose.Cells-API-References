---
title: "Класс ChartPoint"
linktitle: "ChartPoint"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ChartPoint. Инкапсулирует объект, представляющий chartpoint в Go."
type: docs
weight: 200
url: /ru/go-cpp/chartpoint/
---

## ChartPoint class

Представляет одну точку в серии на диаграмме.

```go

type ChartPoint struct  {
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
| [GetExplosion](./getexplosion/) | Расстояние открытого сектора круговой диаграммы от центра выражается в процентах от диаметра круга. |
| [SetExplosion](./setexplosion/) | Расстояние открытого сектора круговой диаграммы от центра выражается в процентах от диаметра круга. |
| [GetShadow](./getshadow/) | Истина, если chartpoint имеет тень. |
| [SetShadow](./setshadow/) | Истина, если chartpoint имеет тень. |
| [GetBorder](./getborder/) | Получает Line</see>. |
| [GetArea](./getarea/) | Получает Area</see>. |
| [GetMarker](./getmarker/) | Получает Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Возвращает объект DataLabels, представляющий подпись данных, связанную с этой точкой диаграммы. |
| [Get_YValue](./get_yvalue/) | Получает или задает значение Y точки диаграммы. |
| [SetYValue](./setyvalue/) | Получает или задает значение Y точки диаграммы. |
| [GetYValueType](./getyvaluetype/) | Получает тип значения Y точки диаграммы. |
| [GetXValue](./getxvalue/) | Получает или задает значение X точки диаграммы. |
| [SetXValue](./setxvalue/) | Получает или задает значение X точки диаграммы. |
| [GetXValueType](./getxvaluetype/) | Получает тип значения X точки диаграммы. |
| [GetShapeProperties](./getshapeproperties/) | Получает объект ShapePropertyCollection, содержащий визуальные свойства формы ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Получает или задает значение, указывающее, находится ли эта точка данных во втором секторе или столбце круговой диаграммы. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Получает или задает значение, указывающее, находится ли эта точка данных во втором секторе или столбце круговой диаграммы. |
| [GetShapeX](./getshapex/) | Получает координату x верхнего левого угла в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [GetShapeY](./getshapey/) | Получает координату y верхнего левого угла в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | Получает ширину в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | Получает высоту в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Получает координату x верхнего левого угла в пикселях после вызова метода Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Получает координату y верхнего левого угла в пикселях после вызова метода Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Получает ширину в пикселях после вызова метода Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Получает высоту в пикселях после вызова метода Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Получает ширину границы в пикселях после вызова метода Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Получает радиус пузыря, сектора или кольца в пикселях после вызова метода Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Получает внутренний радиус сектора кольца в пикселях после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut. |
| [GetStartAngle](./getstartangle/) | Получает начальный угол сектора круговой диаграммы, измеряемый в градусах по часовой стрелке от оси X после вызова метода Chart.Calculate(). Применяется к диаграмме Pie. |
| [GetEndAngle](./getendangle/) | Получает конечный угол сектора круговой диаграммы, измеряемый в градусах по часовой стрелке от оси X после вызова метода Chart.Calculate(). Применяется к диаграмме Pie. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Получает координату x начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Получает координату y начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Получает координату x конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Получает координату y конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Получает координату x начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Получает координату y начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Получает координату x конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к кольцевым диаграммам. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Получает координату y конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate(). Применяется к кольцевой диаграмме. |
| [GetTopPointCount](./gettoppointcount/) | Получает количество верхних точек после вызова метода Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Получает координату x верхней точки фигуры после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D. |
| [GetTopPointYPx](./gettoppointypx/) | Получает координату y верхней точки фигуры после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Получает количество нижних точек после вызова метода Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Получает координату x нижней точки фигуры после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetBottomPointYPx](./getbottompointypx/) | Получает координату y нижней точки фигуры после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Получает количество точек на оси категорий после вызова метода Chart.Calculate(). Применяется только к областным диаграммам. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Получает координату x точки на оси категорий после вызова метода Chart.Calculate(). Применяется только к областной диаграмме. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Получает координату y точки на оси категорий после вызова метода Chart.Calculate(). Применяется только к областной диаграмме. |
