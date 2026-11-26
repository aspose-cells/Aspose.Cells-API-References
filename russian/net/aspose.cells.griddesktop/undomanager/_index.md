---
title: "Класс UndoManager"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridDesktop.UndoManager. Инкапсулирует объект, управляющий операциями отмены/повтора."
type: docs
url: /ru/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

Инкапсулирует объект, управляющий операциями отмены/повтора.

```csharp
public class UndoManager
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled/) { get; set; } | Получает или задает значение, указывающее, включена ли функция отмены. Значение по умолчанию — false. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount/) { get; } | Получает текущее количество доступных шагов повтора. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize/) { get; set; } | Получает или задает размер стека отмены/повтора. Значение по умолчанию — 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount/) { get; } | Получает текущее количество доступных шагов отмены. |

## Методы

| Имя | Описание |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges/)() | Начинает запись изменений. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark/)() | Начинает помечать изменения. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack/)() | Очищает стеки отмены и повтора. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges/)() | Завершает запись изменений. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark/)() | Завершает пометку изменений. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo/)() | Выполняет операцию повтора. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark/)() | Выполняет операцию повтора с пометкой. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo/)() | Выполняет операцию отмены. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark/)() | Выполняет операцию отмены с пометкой. |

### См. также

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


