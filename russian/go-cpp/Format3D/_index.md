---
title: "Класс Format3D"
linktitle: "Format3D"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Format3D. Инкапсулирует объект, представляющий format3d в Go."
type: docs
weight: 200
url: /ru/go-cpp/format3d/
---

## Format3D class

Этот класс задаёт свойства 3D‑формы для элемента диаграммы или формы.

```go

type Format3D struct  {
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
| [GetTopBevel](./gettopbevel/) | Получает объект Bevel, содержащий свойства, связанные с определением фаски на верхней или передней грани фигуры. |
| [HasTopBevelData](./hastopbeveldata/) | Указывает, содержит ли фигура данные о верхней фаске. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | Получает и задает тип материала, который комбинируется со свойствами освещения для получения окончательного внешнего вида фигуры. Значение по умолчанию — PresetMaterialType.WarmMatte. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | Получает и задает тип материала, который комбинируется со свойствами освещения для получения окончательного внешнего вида фигуры. Значение по умолчанию — PresetMaterialType.WarmMatte. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | Получает и задает тип освещения, который будет применён к сцене фигуры. Значение по умолчанию — LightRigType.ThreePoint. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | Получает и задает тип освещения, который будет применён к сцене фигуры. Значение по умолчанию — LightRigType.ThreePoint. |
| [GetLightingAngle](./getlightingangle/) | Получает и задает угол освещения. Диапазон от 0 до 359.9 градусов. |
| [SetLightingAngle](./setlightingangle/) | Получает и задает угол освещения. Диапазон от 0 до 359.9 градусов. |
