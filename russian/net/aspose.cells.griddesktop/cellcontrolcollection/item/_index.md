---
title: Item
second_title: Справочник по Aspose.Cells для .NET API
description: Получает элемент управления ячейкой по указанному индексу строки и столбца.
type: docs
weight: 10
url: /ru/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Получает элемент управления ячейкой по указанному индексу строки и столбца.

```csharp
public CellControl this[int row, int col] { get; }
```

| Параметр | Описание |
| --- | --- |
| row | индекс строки. |
| col | индекс столбца. |

### Примечания

Если нет объекта CellControl в указанном индексе столбца строки, это проверит объект CellControl столбца .

### Смотрите также

* class [CellControl](../../cellcontrol)
* class [CellControlCollection](../../cellcontrolcollection)
* пространство имен [Aspose.Cells.GridDesktop](../../cellcontrolcollection)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Получает элемент управления ячейкой по указанному имени ячейки.

```csharp
public CellControl this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | имя ячейки (в формате имени excel, например 'A1', 'F22') |

### Примечания

Если нет объекта CellControl в указанном индексе столбца строки, будет проверен объект CellControl столбца.

### Смотрите также

* class [CellControl](../../cellcontrol)
* class [CellControlCollection](../../cellcontrolcollection)
* пространство имен [Aspose.Cells.GridDesktop](../../cellcontrolcollection)
* сборка [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->