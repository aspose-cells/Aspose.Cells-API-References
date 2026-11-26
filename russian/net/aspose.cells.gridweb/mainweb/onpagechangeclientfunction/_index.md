---
title: "MainWeb.OnPageChangeClientFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MainWeb. Получает или задает клиентскую функцию, которая будет вызвана после изменения индекса страницы. Действует только когда EnablePaging равно true. Клиентская функция должна быть объявлена так: function MyOnPageChangeindex  console.logcurrent page isindex  Примечание: Вы можете использовать указатель this в клиентской функции, чтобы обратиться к элементу управления сеткой, который генерирует событие"
type: docs
url: /ru/net/aspose.cells.gridweb/mainweb/onpagechangeclientfunction/
---
## MainWeb.OnPageChangeClientFunction property

Получает или задает клиентскую функцию, которая будет вызываться после изменения индекса страницы. Работает только при EnablePaging = true. Клиентская функция должна быть объявлена так: function MyOnPageChange(index) { console.log(\"current page is:\"+index); }Примечание: Вы можете использовать указатель \"this\" в клиентской функции, чтобы указать на элемент управления сеткой, который генерирует событие.

```csharp
public string OnPageChangeClientFunction { get; set; }
```

### См. также

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


