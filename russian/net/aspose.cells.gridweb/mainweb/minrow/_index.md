---
title: "MainWeb.MinRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MainWeb свойство. Получает или задает минимальный индекс строки отображения, начинающийся с нуля, основанный на веб‑листe. Управление использует меньшее значение из MinRow и минимального индекса строки данных листа."
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/minrow/
---
## MainWeb.MinRow property

Получает или задает минимальный индекс отображаемой строки (нумерация с нуля) веб‑листа. Элемент управления использует меньшее значение из MinRow и минимальной строки данных листа.

```csharp
public int MinRow { get; set; }
```

### Примеры

```csharp
[C#]
	// Создаёт 4×4 «окно отображения».
	GridWeb1.MinRow = 2;
	GridWeb1.MaxRow = 5;
	GridWeb1.MinColumn = 3;
	GridWeb1.MaxColumn = 6;

[Visual Basic]
	' Creates a 4x4 "display window".
	GridWeb1.MinRow = 2
	GridWeb1.MaxRow = 5
	GridWeb1.MinColumn = 3
	GridWeb1.MaxColumn = 6
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


