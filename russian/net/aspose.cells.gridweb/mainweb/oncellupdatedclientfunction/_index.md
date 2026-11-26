---
title: "MainWeb.OnCellUpdatedClientFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MainWeb свойство. Получает или задает имя клиентской функции, которая будет вызываться, когда значение ячейки обновляется. Клиентская функция должна быть объявлена так: function MyOnCellUpdatedcell  alertthis.getCellValueByCellcell Примечание: Вы можете использовать указатель this в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие"
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/
---
## MainWeb.OnCellUpdatedClientFunction property

Получает или задает имя клиентской функции, вызываемой при обновлении значения ячейки. Клиентская функция должна быть объявлена так: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

```csharp
public string OnCellUpdatedClientFunction { get; set; }
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


