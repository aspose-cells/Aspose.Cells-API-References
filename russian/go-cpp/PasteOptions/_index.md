---
title: "PasteOptions Класс"
linktitle: "PasteOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PasteOptions класс. Инкапсулирует объект, представляющий pasteoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/pasteoptions/
---

## PasteOptions class

Представляет параметры специальной вставки.

```go

type PasteOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPasteOptions](./newpasteoptions/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetPasteType](./getpastetype/) | Тип специальной вставки. |
| [SetPasteType](./setpastetype/) | Тип специальной вставки. |
| [GetShiftFormulasOfShapes](./getshiftformulasofshapes/) | Указывает, следует ли смещать формулы фигур при копировании диапазонов. |
| [SetShiftFormulasOfShapes](./setshiftformulasofshapes/) | Указывает, следует ли смещать формулы фигур при копировании диапазонов. |
| [GetSkipBlanks](./getskipblanks/) | Указывает, пропускать ли пустые ячейки. |
| [SetSkipBlanks](./setskipblanks/) | Указывает, пропускать ли пустые ячейки. |
| [GetKeepOldTables](./getkeepoldtables/) | Сохраняет таблицы в диапазоне назначения. |
| [SetKeepOldTables](./setkeepoldtables/) | Сохраняет таблицы в диапазоне назначения. |
| [GetOnlyVisibleCells](./getonlyvisiblecells/) | True означает копирование только видимых ячеек. |
| [SetOnlyVisibleCells](./setonlyvisiblecells/) | True означает копирование только видимых ячеек. |
| [GetTranspose](./gettranspose/) | True для транспонирования строк и столбцов при вставке диапазона. Значение по умолчанию — False. |
| [SetTranspose](./settranspose/) | True для транспонирования строк и столбцов при вставке диапазона. Значение по умолчанию — False. |
| [GetOperationType](./getoperationtype/) | Получает и задает тип операции при вставке диапазона. |
| [SetOperationType](./setoperationtype/) | Получает и задает тип операции при вставке диапазона. |
| [GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | Игнорировать ссылки на оригинальный файл. |
| [SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | Игнорировать ссылки на оригинальный файл. |
