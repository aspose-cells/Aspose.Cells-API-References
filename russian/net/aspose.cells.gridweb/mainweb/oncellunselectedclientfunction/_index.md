---
title: OnCellUnselectedClientFunction
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает функцию на стороне клиента которая будет вызываться когда ячейка не выбрана. Клиентская функция должна быть объявлена следующим образомltbr /gt function MyOnUnselectCellcellltbr /gt ltbr /gt GridWeb1.setCellValueByCellcell testltbr /gt ltbr /gtltbr /gtПримечание. Вы можете использовать указатель this в клиентской функции. чтобы указать элемент управления сеткой который запускает событие.
type: docs
weight: 600
url: /ru/net/aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/
---
## MainWeb.OnCellUnselectedClientFunction property

Получает или задает функцию на стороне клиента, которая будет вызываться, когда ячейка не выбрана. Клиентская функция должна быть объявлена следующим образом:&lt;br /&gt; function MyOnUnselectCell(cell)&lt;br /&gt; {&lt;br /&gt; GridWeb1.setCellValueByCell(cell, "test");&lt;br /&gt; }&lt;br /&gt;&lt;br /&gt;Примечание. Вы можете использовать указатель this в клиентской функции. чтобы указать элемент управления сеткой, который запускает событие.

```csharp
public string OnCellUnselectedClientFunction { get; set; }
```

### Смотрите также

* class [MainWeb](../../mainweb)
* пространство имен [Aspose.Cells.GridWeb](../../mainweb)
* сборка [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
