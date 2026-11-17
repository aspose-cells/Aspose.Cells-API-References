---
title: "Перечисление ShapePathType"
linktitle: "ShapePathType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление ShapePathType. Инкапсулирует объект, представляющий shapepathtype в Go."
type: docs
weight: 200
url: /ru/go-cpp/shapepathtype/
---

## ShapePathType Enum

Представляет тип сегмента пути.

```go

type ShapePathType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [LineTo](./lineto/) | Прямой отрезок |
| [CubicBezierCurveTo](./cubicbeziercurveto/) | Кубическая кривая Безье |
| [MoveTo](./moveto/) | Начать новый путь |
| [Close](./close/) | Если начальная POINT и конечная POINT не совпадают, рисуется одиночная прямая линия, соединяющая начальную POINT и конечную POINT пути. |
| [End](./end/) | Конец текущего пути |
| [Escape](./escape/) | Выход |
| [ArcTo](./arcto/) | Дуга |
| [Unknown](./unknown/) | Неизвестно |
