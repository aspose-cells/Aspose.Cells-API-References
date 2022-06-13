---
title: OnGridInitClientFunction
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает имя функции на стороне клиента которая будет вызываться при инициализации сетки. Клиентская функция должна быть объявлена следующим образомltbr /gt function MyOnGridInitgridltbr /gt ltbr /gt alertСетка инициализирована  grid.idltbr /gt ltbr /gtltbr /gtПримечание. Вы можете использовать указатель this в клиентской функции чтобы указать элемент управления сеткой который запускает событие.
type: docs
weight: 650
url: /ru/net/aspose.cells.gridweb/mainweb/ongridinitclientfunction/
---
## MainWeb.OnGridInitClientFunction property

Получает или задает имя функции на стороне клиента, которая будет вызываться при инициализации сетки. Клиентская функция должна быть объявлена следующим образом:&lt;br /&gt; function MyOnGridInit(grid)&lt;br /&gt; {&lt;br /&gt; alert("Сетка инициализирована:" + grid.id);&lt;br /&gt; }&lt;br /&gt;&lt;br /&gt;Примечание. Вы можете использовать указатель "this" в клиентской функции, чтобы указать элемент управления сеткой, который запускает событие.

```csharp
public string OnGridInitClientFunction { get; set; }
```

### Смотрите также

* class [MainWeb](../../mainweb)
* пространство имен [Aspose.Cells.GridWeb](../../mainweb)
* сборка [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->