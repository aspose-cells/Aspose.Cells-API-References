---
title: OnDoubleClickCellClientFunction
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает функцию на стороне клиента которая будет вызываться при двойном щелчке по ячейке. Клиентская функция должна быть объявлена следующим образомltbr /gt function MyOnDoubleClickCellcellltbr /gt ltbr /gt GridWeb1.setCellValueByCellcell testltbr /gt ltbr /gtltbr /gtПримечание. Вы можете использовать указатель this в клиентской функции. чтобы указать элемент управления сеткой который запускает событие.
type: docs
weight: 630
url: /ru/net/aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/
---
## MainWeb.OnDoubleClickCellClientFunction property

Получает или задает функцию на стороне клиента, которая будет вызываться при двойном щелчке по ячейке. Клиентская функция должна быть объявлена следующим образом:&lt;br /&gt; function MyOnDoubleClickCell(cell)&lt;br /&gt; {&lt;br /&gt; GridWeb1.setCellValueByCell(cell, "test");&lt;br /&gt; }&lt;br /&gt;&lt;br /&gt;Примечание. Вы можете использовать указатель this в клиентской функции. чтобы указать элемент управления сеткой, который запускает событие.

```csharp
public string OnDoubleClickCellClientFunction { get; set; }
```

### Смотрите также

* class [MainWeb](../../mainweb)
* пространство имен [Aspose.Cells.GridWeb](../../mainweb)
* сборка [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
