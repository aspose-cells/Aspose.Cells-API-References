---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MainWeb. Получает или задает клиентскую функцию, вызываемую при отображении контекстного меню. Клиентскую функцию следует объявить так: function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Примечание: Вы можете использовать указатель this в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие."
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Получает или задает клиентскую функцию, которая будет вызываться при отображении контекстного меню. Клиентская функция должна быть объявлена так: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility(\"Delete\", \"block\"); menu.setItemVisibility(\"Update\", \"none\"); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


