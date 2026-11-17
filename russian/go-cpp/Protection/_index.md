---
title: "Protection Класс"
linktitle: "Protection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Protection class. Инкапсулирует объект, представляющий protection в Go."
type: docs
weight: 200
url: /ru/go-cpp/protection/
---

## Protection class

Представляет различные типы параметров защиты, доступные для листа.

```go

type Protection struct  {
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
| [Copy](./copy/) | Скопировать информацию о защите. |
| [GetAllowDeletingColumn](./getallowdeletingcolumn/) | Отображает, разрешено ли удаление столбцов на защищённом листе. |
| [SetAllowDeletingColumn](./setallowdeletingcolumn/) | Отображает, разрешено ли удаление столбцов на защищённом листе. |
| [GetAllowDeletingRow](./getallowdeletingrow/) | Отображает, разрешено ли удаление строк на защищённом листе. |
| [SetAllowDeletingRow](./setallowdeletingrow/) | Отображает, разрешено ли удаление строк на защищённом листе. |
| [GetAllowFiltering](./getallowfiltering/) | Отображает, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа. |
| [SetAllowFiltering](./setallowfiltering/) | Отображает, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа. |
| [GetAllowFormattingCell](./getallowformattingcell/) | Отображает, разрешено ли форматирование ячеек на защищённом листе. |
| [SetAllowFormattingCell](./setallowformattingcell/) | Отображает, разрешено ли форматирование ячеек на защищённом листе. |
| [GetAllowFormattingColumn](./getallowformattingcolumn/) | Отображает, разрешено ли форматирование столбцов на защищённом листе |
| [SetAllowFormattingColumn](./setallowformattingcolumn/) | Отображает, разрешено ли форматирование столбцов на защищённом листе |
| [GetAllowFormattingRow](./getallowformattingrow/) | Отображает, разрешено ли форматирование строк на защищённом листе |
| [SetAllowFormattingRow](./setallowformattingrow/) | Отображает, разрешено ли форматирование строк на защищённом листе |
| [GetAllowInsertingColumn](./getallowinsertingcolumn/) | Отображает, разрешено ли вставка столбцов на защищённом листе |
| [SetAllowInsertingColumn](./setallowinsertingcolumn/) | Отображает, разрешено ли вставка столбцов на защищённом листе |
| [GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | Отображает, разрешено ли вставка гиперссылок на защищённом листе |
| [SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | Отображает, разрешено ли вставка гиперссылок на защищённом листе |
| [GetAllowInsertingRow](./getallowinsertingrow/) | Отображает, разрешено ли вставка строк на защищённом листе |
| [SetAllowInsertingRow](./setallowinsertingrow/) | Отображает, разрешено ли вставка строк на защищённом листе |
| [GetAllowSorting](./getallowsorting/) | Отображает, разрешена ли опция сортировки на защищённом листе. |
| [SetAllowSorting](./setallowsorting/) | Отображает, разрешена ли опция сортировки на защищённом листе. |
| [GetAllowUsingPivotTable](./getallowusingpivottable/) | Отображает, разрешено ли пользователю управлять сводными таблицами на защищённом листе. |
| [SetAllowUsingPivotTable](./setallowusingpivottable/) | Отображает, разрешено ли пользователю управлять сводными таблицами на защищённом листе. |
| [GetAllowEditingContent](./getalloweditingcontent/) | Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе. |
| [SetAllowEditingContent](./setalloweditingcontent/) | Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе. |
| [GetAllowEditingObject](./getalloweditingobject/) | Представляет, разрешено ли пользователю манипулировать объектами рисования на защищённом листе. |
| [SetAllowEditingObject](./setalloweditingobject/) | Представляет, разрешено ли пользователю манипулировать объектами рисования на защищённом листе. |
| [GetAllowEditingScenario](./getalloweditingscenario/) | Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе. |
| [SetAllowEditingScenario](./setalloweditingscenario/) | Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе. |
| [GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе. |
| [SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе. |
| [GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе. |
| [SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе. |
| [GetPassword](./getpassword/) | Представляет пароль для защиты листа. |
| [SetPassword](./setpassword/) | Представляет пароль для защиты листа. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Указывает, защищён ли лист паролем. |
| [VerifyPassword](./verifypassword/) | Проверяет пароль. |
| [GetPasswordHash](./getpasswordhash/) | Получает хеш текущего пароля. |
