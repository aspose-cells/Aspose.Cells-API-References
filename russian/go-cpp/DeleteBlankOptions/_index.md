---
title: "DeleteBlankOptions Класс"
linktitle: "DeleteBlankOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "DeleteBlankOptions class. Инкапсулирует объект, представляющий deleteblankoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Представляет настройку удаления пустых ячеек/строк/столбцов.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Конструктор по умолчанию. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Указывает, будет ли одна ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию: true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Указывает, будет ли одна ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию: true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Будет ли одна ячейка считаться пустой, когда это формула, а вычисленный результат — null или пустая строка. Значение по умолчанию: false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Будет ли одна ячейка считаться пустой, когда это формула, а вычисленный результат — null или пустая строка. Значение по умолчанию: false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Указывает, будут ли объекты, связанные с рисунками, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию: true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Указывает, будут ли объекты, связанные с рисунками, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию: true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов. |
| [GetStartIndex](./getstartindex/) | Указывает начальный индекс строки/столбца диапазона, который следует проверить и удалить пустые строки/столбцы. |
| [SetStartIndex](./setstartindex/) | Указывает начальный индекс строки/столбца диапазона, который следует проверить и удалить пустые строки/столбцы. |
| [GetEndIndex](./getendindex/) | Указывает конечный индекс строки/столбца (включительно) диапазона, который следует проверить и удалить пустые строки/столбцы. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячейки, рисунки, ...) которые необходимо проверить. |
| [SetEndIndex](./setendindex/) | Указывает конечный индекс строки/столбца (включительно) диапазона, который следует проверить и удалить пустые строки/столбцы. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячейки, рисунки, ...) которые необходимо проверить. |
| [GetUpdateReference](./getupdatereference/) | Указывает, обновлять ли ссылки в других листах. |
| [SetUpdateReference](./setupdatereference/) | Указывает, обновлять ли ссылки в других листах. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Получает/устанавливает монитор для отслеживания изменений, вызванных удалением. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Получает/устанавливает монитор для отслеживания изменений, вызванных удалением. |
