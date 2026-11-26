---
title: "MainWeb.OnCellErrorClientFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MainWeb. Получает или задает имя клиентской функции, вызываемой при ошибке проверки ячейки. Клиентская функция должна быть объявлена так: function MyOnCellErrorcell  alertthis.getCellValueByCellcell. Примечание: вы можете использовать указатель this в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие."
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/oncellerrorclientfunction/
---
## MainWeb.OnCellErrorClientFunction property

Получает или задает имя клиентской функции, вызываемой при ошибке проверки ячейки. Клиентская функция должна быть объявлена так: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Примечание: вы можете использовать указатель \"this\" в клиентской функции, чтобы ссылаться на элемент управления сеткой, который генерирует событие.

```csharp
public string OnCellErrorClientFunction { get; set; }
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


