---
title: "Класс CustomCommandButtonCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.CustomCommandButtonCollection class. Представляет коллекцию CustomCommandButton"
type: docs
url: /ru/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Представляет коллекцию CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Возвращает количество элементов коллекции. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Используется только внутри. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Используется только внутри. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Используется только внутри. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Получает объект пользовательской кнопки команды по индексу. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Используется только внутри. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Добавляет объект пользовательской кнопки команды в коллекцию. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Очищает коллекцию. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Указывает, находится ли объект пользовательской кнопки команды в коллекции. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Копирует коллекцию в массив. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Получает объект IEnumerator коллекции. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Получает индекс кнопки. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | Вставляет кнопку по индексу. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Удаляет объект пользовательской кнопки команды. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | Удаляет по индексу. |

### Примеры

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim GridWeb1 As GridWeb= New GridWeb();
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### См. также

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


