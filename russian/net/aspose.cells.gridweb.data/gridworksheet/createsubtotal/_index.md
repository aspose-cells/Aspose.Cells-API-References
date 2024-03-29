---
title: CreateSubtotal
second_title: Справочник по Aspose.Cells для .NET API
description: Создает промежуточный итог на листе.
type: docs
weight: 490
url: /ru/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

Создает промежуточный итог на листе.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Индекс строки имени столбца row. |
| dataRows | Int32 | Количество строк данных. |
| groupByColumnIndex | Int32 | Индекс столбца для группируемого столбца. |
| subtotalFunction | SubtotalFunction | Тип функции промежуточного итога. |
| subtotalColumnIndexList | Int32[] | Индексы столбца для промежуточного итога. |
| functionLabel | String | Метка функции промежуточного итога. |
| grandCellStyle | GridTableItemStyle | Стиль общей линии. |
| subtotalCellStyle | GridTableItemStyle | Стиль строки промежуточного итога. |
| numberType | NumberType | Числовой тип ячеек результата промежуточного итога. |
| customString | String | Строка пользовательского формата ячеек результатов промежуточных итогов. Может быть нулевым. |

### Смотрите также

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle)
* enum [NumberType](../../numbertype)
* class [GridWorksheet](../../gridworksheet)
* пространство имен [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* сборка [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

Создает промежуточный итог на листе.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Индекс строки имени столбца row. |
| dataRows | Int32 | Количество строк данных. |
| groupByColumnIndex | Int32 | Индекс столбца для группируемого столбца. |
| subtotalFunction | SubtotalFunction | Тип функции промежуточного итога. |
| subtotalColumnIndexList | Int32[] | Индексы столбца для промежуточного итога. |

### Смотрите также

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridWorksheet](../../gridworksheet)
* пространство имен [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* сборка [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
