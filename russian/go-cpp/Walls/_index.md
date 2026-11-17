---
title: "Класс Walls"
linktitle: "Стены"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Walls. Инкапсулирует объект, представляющий стены в Go."
type: docs
weight: 200
url: /ru/go-cpp/walls/
---

## Walls class

Инкапсулирует объект, представляющий стены 3‑D диаграммы.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewWalls](./newwalls/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetCenterX](./getcenterx/) | Получает координату x левого нижнего угла центра стены в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [GetCenterY](./getcentery/) | Получает координату y левого нижнего угла центра стены в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [GetWidth](./getwidth/) | Получает ширину слева направо в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [GetDepth](./getdepth/) | Получает глубину спереди назад в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [GetHeight](./getheight/) | Получает высоту сверху вниз в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [GetCenterXPx](./getcenterxpx/) | Получает координату x нижнего левого угла центра стены в пикселях после вызова метода Chart.Calculate(). |
| [GetCenterYPx](./getcenterypx/) | Получает координату y левого нижнего угла центра стены в пикселях после вызова метода Chart.Calculate(). |
| [GetWidthPx](./getwidthpx/) | Получает ширину слева направо в пикселях после вызова метода Chart.Calculate(). |
| [GetDepthPx](./getdepthpx/) | Получает глубину спереди назад в пикселях после вызова метода Chart.Calculate(). |
| [GetHeightPx](./getheightpx/) | Получает высоту сверху вниз в пикселях после вызова метода Chart.Calculate(). |
| [GetCubePointCount](./getcubepointcount/) | Получает количество точек куба после вызова метода Chart.Calculate(). |
| [GetCubePointXPx](./getcubepointxpx/) | Получает координату x вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми. |
| [GetCubePointYPx](./getcubepointypx/) | Получает координату y вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми. |
| [GetBackgroundColor](./getbackgroundcolor/) | Получает или задает фоновый Color области. |
| [SetBackgroundColor](./setbackgroundcolor/) | Получает или задает фоновый Color области. |
| [GetForegroundColor](./getforegroundcolor/) | Получает или задает передний Color. |
| [SetForegroundColor](./setforegroundcolor/) | Получает или задает передний Color. |
| [GetFormatting](./getformatting/) | Представляет форматирование области. |
| [SetFormatting](./setformatting/) | Представляет форматирование области. |
| [GetInvertIfNegative](./getinvertifnegative/) | Если свойство истинно и значение точки диаграммы отрицательное, передний цвет и фоновый цвет будут обменены. |
| [SetInvertIfNegative](./setinvertifnegative/) | Если свойство истинно и значение точки диаграммы отрицательное, передний цвет и фоновый цвет будут обменены. |
| [GetFillFormat](./getfillformat/) | Представляет объект FillFormat, содержащий свойства форматирования заливки для указанной диаграммы или фигуры. |
| [GetTransparency](./gettransparency/) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [SetTransparency](./settransparency/) | Возвращает или задает степень прозрачности области значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [GetBorder](./getborder/) | Получает или задает границу Line. |
| [SetBorder](./setborder/) | Получает или задает границу Line. |
