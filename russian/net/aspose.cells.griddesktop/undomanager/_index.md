---
title: UndoManager
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект управляющий операциями отмены/возврата.
type: docs
weight: 1030
url: /ru/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

Инкапсулирует объект, управляющий операциями отмены/возврата.

```csharp
public class UndoManager
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled) { get; set; } | Получает или задает значение, указывающее, включена ли функция отмены. Значение по умолчанию неверно. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount) { get; } | Получает текущее количество доступных повторных шагов. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize) { get; set; } | Получает или задает размер стека отмены/возврата. Значение по умолчанию — 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount) { get; } | Получает текущее количество доступных шагов отмены. |

## Методы

| Имя | Описание |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges)() | Начинает записывать изменения. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark)() | Начинает отмечать изменения. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack)() | Очищает стеки Undo и Redo. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges)() | Заканчивается записью изменений. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark)() | Заканчивается, чтобы отметить изменения. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo)() | Выполняет операцию повтора. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark)() | Выполняет операцию повтора с пометкой. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo)() | Выполняет операцию отмены. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark)() | Выполняет операцию отмены с пометкой. |

### Смотрите также

* пространство имен [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->