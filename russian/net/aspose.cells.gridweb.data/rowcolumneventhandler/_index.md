---
title: "Делегат RowColumnEventHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Представляет интерфейс, предназначенный для обработки событий строк/столбцов"
type: docs
url: /ru/net/aspose.cells.gridweb.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Представляет интерфейс, предназначенный для обработки событий строк/столбцов.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | Object | Источник события. |
| e | RowColumnEventArgs | Аргумент события. Вызовите e.RejectOperation(), если хотите отменить операцию удаления в обработчиках событий RowDeleting или ColumnDeleting. |

### См. также

* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


