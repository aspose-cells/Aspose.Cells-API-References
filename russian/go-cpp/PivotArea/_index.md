---
title: "Класс PivotArea"
linktitle: "PivotArea"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotArea. Инкапсулирует объект, представляющий pivotarea в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotarea/
---

## PivotArea class

Отображает выбранную область сводной таблицы.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | Отображает выбранную область PivotTable. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetFilters](./getfilters/) | Получает все фильтры для этого PivotArea. |
| [Select](./select/) | Выберите область с фильтрами. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Выберите поле в регионе в качестве области. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Выберите поле в регионе в качестве области. |
| [GetOnlyData](./getonlydata/) | Указывает, выбраны ли только значения данных (в области данных представления) для itemselection и не включают метки элементов. |
| [SetOnlyData](./setonlydata/) | Указывает, выбраны ли только значения данных (в области данных представления) для itemselection и не включают метки элементов. |
| [GetOnlyLabel](./getonlylabel/) | Указывает, выбраны ли только подписи данных для выбора элемента. |
| [SetOnlyLabel](./setonlylabel/) | Указывает, выбраны ли только подписи данных для выбора элемента. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Указывает, включён ли общий итог по строкам. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Указывает, включён ли общий итог по строкам. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Указывает, включён ли общий итог по столбцам. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Указывает, включён ли общий итог по столбцам. |
| [GetAxisType](./getaxistype/) | Получает и задаёт регион PivotTable, к которому применяется это правило. |
| [SetAxisType](./setaxistype/) | Получает и задаёт регион PivotTable, к которому применяется это правило. |
| [GetRuleType](./getruletype/) | Получает и задает тип правила выбора. |
| [SetRuleType](./setruletype/) | Получает и задает тип правила выбора. |
| [IsOutline](./isoutline/) | Указывает, относится ли правило к области, находящейся в режиме контура. |
| [SetIsOutline](./setisoutline/) | Указывает, относится ли правило к области, находящейся в режиме контура. |
| [GetCellAreas](./getcellareas/) | Получает области ячеек этой сводной области. |
